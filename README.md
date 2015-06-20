How to use this code:

1. Copy the code to a new application called "doorStatus" on your spark/particle core. To do this copy the code in the github file called "core"  then go to: https://build.particle.io select your core then paste the code into a new app.
2. This code uses the HttpClient library. Load this library from inside build.particle.io
3. You will need an Ubidots account. Set one up here:  http://app.ubidots.com/accounts/signup/
4. On Ubidots create a new datasource and two variables one digital "isClosed" and one analog called "analog". Copy the IDs for these variables into the main code. 

//These values come from Ubidots.
#define VARIABLE_ID "UBIDOTS_ID123abc"
#define VARIABLE_ID_analog "2ND_UBIDOTS_ID123abc" 

5. Under "profile" on Ubidots create and then copy an new access token. Paste it  into the main code after the variable_ids.

#define TOKEN "superSecrectToken123abc"

6. Flash the new code to your particle core.
7. Use the wiring diagrams: http://www.hackster.io/futurebird/simple-door-sensor  to get everything connected.

