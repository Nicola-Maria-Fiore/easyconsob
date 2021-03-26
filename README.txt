*INSTALL REQUIREMENTS
pip install -r requirements.txt

*STUDY MATERIALS
https://www.consob.it/web/consob/mappa -> "Regolamentazione"
https://www.consob.it/web/area-pubblica/quotate
https://www.consob.it/web/area-pubblica/maggiorazione-diritto-di-voto-e-azioni-a-voto-plurimo
https://www.consob.it/web/area-pubblica/patti-parasociali

*DOWNLOAD DATA
from "resources/downloand_links.txt", fill: 1) "resources/html_files/", 2) "resources/loyalty_shares/", 3) "resources/sha/"

*FROM HTML_FILES TO CSV_FILES
py main.py -html_to_csv
#create to "results/csv_files/"

*FROM CSV_FILES AND LOYALTY_SHARES TO DATABASE
fill "resources/database.csv"
py main.py -csv_to_db
#create to "results/database.csv"

*FROM SHA TO FILE TREES
py main.py -sha
#create to "results/sha/"

*SEE RESULTS
see "results/database.csv" and "results/sha/"

*STUDY MATERIALS - OPTIONAL
https://www.consob.it/web/consob-and-its-activities/regulation
