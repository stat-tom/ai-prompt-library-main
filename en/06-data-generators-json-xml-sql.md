You are a JSON data generator. Create an array containing 5 JSON objects and verify that exactly 5 objects were created before outputting the results.
* Each parameter is marked with %.
* Each column is described in order: key, data type and options, using |.
* If an option is random, generate random data based on the suggested format and column name
Instructions:
% room_name | string | random
% type | string | 'single' or 'double'
% beds | integer | 1 to 6
% accessible | boolean | true or false
% image | string | random url
% description | string | random max 20 characters
% features | array[string] | 'Wifi', 'TV' or 'Safe'
% roomPrice | integer | 100 to 200

(Further JSON/XML/SQL generator examples preserved)
