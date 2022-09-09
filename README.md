# Apex-Legends-Weapon-Stats-API
This is an API that will provide you with stats and information on weapons from Apex Legends.

## 🛑🤚 Before you continue
This is an ongoing project and takes a lot of time to create. Some weapons are missing and some stats are missing. I am not done with it yet and I am doing my best to get it done. Thank you for understanding!

# 🔥 Usage
Here is the link to RapidApi where you can get your API key. [Get Access!](https://rapidapi.com/ItsSpres/api/apex-legends-weapon-stats1)

###### 🧑‍💻 Javascript Use
```
const settings = {
	"async": true,
	"crossDomain": true,
	"url": "https://apex-legends-weapon-stats1.p.rapidapi.com/weapons",
	"method": "GET",
	"headers": {
		"X-RapidAPI-Key": "YOUR-API-KEY",
		"X-RapidAPI-Host": "apex-legends-weapon-stats1.p.rapidapi.com"
	}
};

$.ajax(settings).done(function (response) {
	console.log(response);
});
```
###### 🍎 Swift Use
```
import Foundation

let headers = [
	"X-RapidAPI-Key": "YOUR-API-KEY",
	"X-RapidAPI-Host": "apex-legends-weapon-stats1.p.rapidapi.com"
]

let request = NSMutableURLRequest(url: NSURL(string: "https://apex-legends-weapon-stats1.p.rapidapi.com/weapons")! as URL,
                                        cachePolicy: .useProtocolCachePolicy,
                                    timeoutInterval: 10.0)
request.httpMethod = "GET"
request.allHTTPHeaderFields = headers

let session = URLSession.shared
let dataTask = session.dataTask(with: request as URLRequest, completionHandler: { (data, response, error) -> Void in
	if (error != nil) {
		print(error)
	} else {
		let httpResponse = response as? HTTPURLResponse
		print(httpResponse)
	}
})

dataTask.resume()
```
###### 🐍 Python Use
```
import requests

url = "https://apex-legends-weapon-stats1.p.rapidapi.com/weapons"

headers = {
	"X-RapidAPI-Key": "d842a2d802mshcc69a70064149a4p17ebd2jsnc20dce5ed8bc",
	"X-RapidAPI-Host": "apex-legends-weapon-stats1.p.rapidapi.com"
}

response = requests.request("GET", url, headers=headers)

print(response.text)
```
# Response
This is not the whole response but feel free to check out this file. 
[API Response(JSON)](docs/weaponsJson.json)
