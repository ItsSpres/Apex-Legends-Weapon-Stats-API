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
This is not the whole response.
```
{
  "Weapons": {
    "Assault": [
      {
        "Name": "R301 Carbine",
        "isWeaponinSupplyDrop": false,
        "WeaponImage": "no url",
        "Type": "Light Rounds",
        "AmmoImage": "no url",
        "FireModes": [
          "Auto",
          "Single"
        ],
        "Manufacturer": "Lastimosa Armory",
        "AttachmentSlots": [
          "Barrel Stabilizer",
          "Extended Light Magazine",
          "Optics",
          "Standard Stock"
        ],
        "BodyDamage": {
          "name": "14",
          "value": 14
        },
        "HeadDamage": {
          "name": "25(1.75x)",
          "value": 25
        },
        "LegDamage": {
          "name": "11(0.75x)",
          "value": 11
        },
        "RPM": "810",
        "DPS": "189",
        "MagazineSize": {
          "normal": "18",
          "gray": "20",
          "blue": "25",
          "purple": "28"
        },
        "TacReloadTime": {
          "normal": "2.4",
          "gray": "2.32",
          "blue": "2.24",
          "purple": "2.16"
        },
        "FullReloadTime": {
          "normal": "3.2",
          "gray": "3.09",
          "blue": "2.99",
          "purple": "2.88"
        },
        "Attachments": {
          "Optics": [
            "1x HCOG 'Classic'",
            "1x Holo",
            "1x-2x Variable Holo",
            "2x HCOG 'Bruiser'",
            "3x HCOG 'Ranger'",
            "2x-4x Variable AOG"
          ],
          "BarrelStabilizer": [
            "Common",
            "Rare",
            "Epic"
          ],
          "ExtendedLightMag": [
            "Common",
            "Rare",
            "Epic",
            "Legendary"
          ],
          "StandardStock": [
            "Common",
            "Rare",
            "Epic"
          ]
        },
        "WeaponSkins": "Coming soon!"
      }
    ],
    "SMG": [
      {
        "Name": "R-99 SMG"
      }
    ]
  }
}
```
