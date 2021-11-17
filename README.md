# JSON scheme pulu project

In this repository you find a JSON scheme for the TTN listener of the pulu project

## Information

This JSON schema will check if the JSON object that comes from TheThingsNetwork is correctly formatted. Below you see the structure of the JSON object.

## Structure of JSON object

First we will have a main attribute that names "sensors". In this attribute you will find all the information of the sensors. This will have several sub-attributes with specific values in it. We have four different attributes that each correspond to a specific TYPE of sensor. The different types we have are moisture, light, voltage and temperature. Within these types we will find every individual sensor of the project. Each sensor has two attributes. One that has the value of the sensor in it and one that has a status code in it. The status attribute is not necessary for the JSON schema.

## Status codes

The status codes aren't implemented yet. For the moment we don't send a status for each sensor.

## Changelogs

Below you see all the things that have been changed in the different versions of the schema.

### V1.4

* Added the posibility to add a state attribute to each sensor.

### V1.5

* Fixed bug that you can add as many attributes as you want.

### V2.0

* Added control over the values. Minimum and maximum values.

### V2.1

* Small change to make the object a little clearer.

### V2.2

* Changed the amount of moisture sensors to 4 instead of 8.

### V2.3

* Changed the minimum and maximum values of temperature sensors to match real values of datasheet.
