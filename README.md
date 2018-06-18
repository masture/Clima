# Clima

This App access users current location with his permission and then fetches the current temperature from openweathermap.org.
It allows user to display the temperature either in Centigrade or Fahrenheit.
Also user can enter a city and get its temperature.
A large image changes as per the whether like Cloudy, Sunny, Snow, Storm, etc.
The images and included as part of the App bundle and are included in Images.xassets.


## Fix for App Transport Security Override

```XML
	<key>NSAppTransportSecurity</key>
	<dict>
		<key>NSExceptionDomains</key>
		<dict>
			<key>openweathermap.org</key>
			<dict>
				<key>NSIncludesSubdomains</key>
				<true/>
				<key>NSTemporaryExceptionAllowsInsecureHTTPLoads</key>
				<true/>
			</dict>
		</dict>
	</dict>
```
