[![](https://scdn.rapidapi.com/RapidAPI_banner.png)](https://rapidapi.com/package/AccuWeather/functions?utm_source=RapidAPIGitHub_AccuWeatherFunctions&utm_medium=button&utm_content=RapidAPI_GitHub)

# AccuWeather Package
AccuWeather provides hourly and Minute by Minute™ forecasts with Superior Accuracy™ for any longitude/latitude on Earth, with customized content and engaging video presentations available on smart phones, tablets, free wired and mobile Internet sites, connected TVs, and Internet appliances, as well as via radio, television, and newspapers.
* Domain: [AccuWeather](http://accuweather.com/)
* Credentials: apiKey

## How to get credentials: 
0. Go to [AccuWeather](https://developer.accuweather.com) 
1. Register or log in
2. Create new application at [Application page](https://developer.accuweather.com/user/me/apps)

## Custom datatypes: 
 |Datatype|Description|Example
 |--------|-----------|----------
 |Datepicker|String which includes date and time|```2016-05-28 00:00:00```
 |Map|String which includes latitude and longitude coma separated|```50.37, 26.56```
 |List|Simple array|```["123", "sample"]``` 
 |Select|String with predefined values|```sample```
 |Array|Array of objects|```[{"Second name":"123","Age":"12","Photo":"sdf","Draft":"sdfsdf"},{"name":"adi","Second name":"bla","Age":"4","Photo":"asfserwe","Draft":"sdfsdf"}] ```
 

## AccuWeather.listAdminAreas
Returns basic information about administrative areas in the specified country.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Country code
| language   | Select     | String indicating the language in which to return the resource
| offset     | Number     | Integer, along with the limit (25) that determines the first resource to be returned.

## AccuWeather.listCountries
Returns basic information about all countries within a specified region.

| Field     | Type       | Description
|-----------|------------|----------
| apiKey    | credentials| Your API key
| regionCode| String     | Region code
| language  | Select     | String indicating the language in which to return the resource

## AccuWeather.listRegions
Returns basic information about all regions.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.listTopCities
Returns information for the top 50, 100, or 150 cities, worldwide.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| group   | Number     | Integer value (50, 100, or 150) that specifies the number of cities to return
| language| Select     | String indicating the language in which to return the resource
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchLocations
Returns basic information about locations matching an autocomplete of the search text.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| query   | String     | Text to search for.
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.getNeighborCitiesByLocationKey
Returns information about neighboring cities, by location key.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchByLocationKey
Returns information about a specific location, by location key. 

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchCity
Returns information for an array of cities that match the search text.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| query   | String     | Text to search for.
| language| Select     | String indicating the language in which to return the resource
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset  | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias   | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchCityWithAdminCode
Returns information for an array of cities that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| adminCode  | String     | Code of administrative territory
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset     | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias      | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchCityWithCountryCode
Returns information for an array of cities that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset     | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias      | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchPoi
Returns information for an array of Points of Interest that match the search text.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| query   | String     | Text to search for.
| language| Select     | String indicating the language in which to return the resource
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchPoiWithAdminCode
Returns information for an array of pois that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| adminCode  | String     | Code of administrative territory
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchPoiWithCountryCode
Returns information for an array of pois that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchPostalCode
Returns information for an array of postal codes that match the search text.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| query   | String     | Text to search for.
| language| Select     | String indicating the language in which to return the resource
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchPostalCodeWithCountryCode
Returns information for an array of postal codes that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.searchLocation
Returns information for an array of locations that match the search text.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| query   | String     | Text to search for.
| language| Select     | String indicating the language in which to return the resource
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset  | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias   | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchLocationWithAdminCode
Returns information for an array of locations that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| adminCode  | String     | Code of administrative territory
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset     | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias      | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchLocationWithCountryCode
Returns information for an array of locations that match the search text.

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| countryCode| String     | Code of country
| query      | String     | Text to search for.
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| offset     | Number     | Integer, along with the limit (25) that determines the first resource to be returned.
| alias      | Select     | Enumeration that specifies when alias locations should be included in the results. By default, an alias will only be returned if no official match for the search text was found. Enumeration values: Never or Always

## AccuWeather.searchByGeoposition
Returns information about a specific location, by GeoPosition (Latitude and Longitude).

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| coordinates| Map        | Text to search for. In this case, the text should be a comma-separated lat/lon pair (lat,lon).
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| toplevel   | Select     | When toplevel=true, the city with the highest rank will be returned. Large cities have higher rank than the neighborhoods within them, so toplevel=true delivers a more generic location result. (Example: 40.73,-74.00 returns Greenwich Village, NY when toplevel=false. If toplevel=true, the same lat/lon pair will return New York, NY.)

## AccuWeather.searchByIp
Returns information about a specific location, by IP Address.

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| ipAddress| String     | Text to search for. In this case, the text should be a valid ip address.
| language | Select     | String indicating the language in which to return the resource
| details  | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getDailyForecastByLocationKey
Daily Forecasts By Location Key

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| days       | Select     | Number of days to get forecast for
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| metric     | Select     | Boolean value (true or false) that specifies to return the data in either metric (=true) or imperial units 

## AccuWeather.getHoursForecastByLocationKey
Hourly Forecasts By Location Key

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| hours      | Select     | Number of hours to get forecast for
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object
| metric     | Select     | Boolean value (true or false) that specifies to return the data in either metric (=true) or imperial units 

## AccuWeather.getCurrentConditionsByLocationKey
Current Conditions By LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.get6HoursConditionsByLocationKey
Historical Current Conditions (past 6 hours) By LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.get24HoursConditionsByLocationKey
Historical Current Conditions (past 24 hours) By LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getCurrentConditionsForTopCities
Current Conditions for Top Cities

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| language| Select     | String indicating the language in which to return the resource
| group   | Number     | Integer value (50, 100, or 150) that specifies the number of cities to return
| details | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getLocationIndicesByGroupId
Daily Indices By LocationKey and GroupId

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| days       | Select     | Days for get indice for
| groupId    | String     | Unique ID used to search for a specific group
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getLocationIndicesByIndexId
Daily Indices By LocationKey and IndexId

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| days       | Select     | Days for get indice for
| indexId    | String     | Unique ID used to search for a specific index
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getLocationIndicesByLocationKey
Daily Indices By LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| days       | Select     | Days for get indice for
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.listDailyIndices
Metadata List of Daily Indices

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.listDailyIndicesGroups
Metadata List of Index Groups

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.getIndicesByGroupId
Metadata List of Indices in a Specific Group

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| groupId | String     | Unique ID used to search for a specific group
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.getSingleIndice
Returns metadata for a specific index type.

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| indiceId| String     | Unique ID used to search for a specific indice
| language| Select     | String indicating the language in which to return the resource

## AccuWeather.getWeatherAlarmByLocationKey
DailyWeather Alarms By Location Key 

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| days       | Select     | Days for get indice for
| language   | Select     | String indicating the language in which to return the resource

## AccuWeather.getAlertsByLocationKey
Alerts By LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| details    | Select     | Boolean value (true or false) that specifies whether or not to include a truncated version of the current conditions object or the full object

## AccuWeather.getImagesByLocationKey
Radar and Satellite Images by LocationKey

| Field      | Type       | Description
|------------|------------|----------
| apiKey     | credentials| Your API key
| locationKey| String     | Unique ID used to search for a specific location
| language   | Select     | String indicating the language in which to return the resource
| resolution | Select     | Available resolutions: 480x480, 640x480, 1024x1024

## AccuWeather.getSingleCyclone
Get cyclone information

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| basinId  | Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| cycloneId| Number     | Numeric id of the tropical cyclone
| year     | DatePicker | Date in format yyyy

## AccuWeather.listCyclonesByYear
Returns basic information about tropical cyclones for a specific year and basin.

| Field  | Type       | Description
|--------|------------|----------
| apiKey | credentials| Your API key
| basinId| Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| year   | DatePicker | Date in format yyyy

## AccuWeather.getSingleActiveCyclone
Returns basic information about a specific tropical cyclone that is currrently active in the specified basin.

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| basinId  | Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| cycloneId| Number     | Numeric id of the tropical cyclone

## AccuWeather.listActiveCyclonsByBasin
Returns basic information about tropical cyclones that are currrently active in the specified basin.

| Field  | Type       | Description
|--------|------------|----------
| apiKey | credentials| Your API key
| basinId| Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )

## AccuWeather.listActiveCyclons
Returns basic information about tropical cyclones that are currrently active

| Field | Type       | Description
|-------|------------|----------
| apiKey| credentials| Your API key

## AccuWeather.getSingleCycloneForecast
Returns all recorded forecast information for a specific tropical cyclone.

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| basinId  | Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| cycloneId| Number     | Numeric id of the tropical cyclone
| year     | DatePicker | Date in format yyyy

## AccuWeather.listSingleCyclonePositions
Returns all recorded position information for a specific tropical cyclone

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| basinId  | Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| cycloneId| Number     | Numeric id of the tropical cyclone
| year     | DatePicker | Date in format yyyy

## AccuWeather.getSingleCyclonePosition
Returns current (most recently updated) position information for a specific tropical cyclone.

| Field    | Type       | Description
|----------|------------|----------
| apiKey   | credentials| Your API key
| basinId  | Select     | Unique id used to identify a basin (NP, SP, NI, SI, AL, EP )
| cycloneId| Number     | Numeric id of the tropical cyclone
| year     | DatePicker | Date in format yyyy

## AccuWeather.listLanguages
List all Languages

| Field | Type       | Description
|-------|------------|----------
| apiKey| credentials| Your API key

## AccuWeather.listTranslationGroups
List of Available Translation Groups

| Field | Type       | Description
|-------|------------|----------
| apiKey| credentials| Your API key

## AccuWeather.getSingleGroupTranslations
List of Translations for a Specific Group

| Field   | Type       | Description
|---------|------------|----------
| apiKey  | credentials| Your API key
| groupId | String     | Unique ID of a translation group
| language| Select     | String indicating the language in which to return the resource

