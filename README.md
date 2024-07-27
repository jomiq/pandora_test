# Pandora test
Skiss till UI:t för endpoint `/upload` där användaren väljer vilka arter som ska kopplas till dokumentet.
Tanke: spara endast referens till artdatas `taxonId` i databasen och hämta infon dynamiskt. 

- Använder [autocomplete.js](https://tarekraafat.github.io/autoComplete.js/) (första vettiga jag hittade)
- Data hämtas från artdatabankens `/information/v1/speciesdataservice/v1/speciesdata/search`
- `get_list()` är en stub för hur jag tänker att fältet kan genereras (lista av `int`)