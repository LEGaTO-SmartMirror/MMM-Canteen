# MMM-Canteen

MMM-Canteen is a module for the [MagicMirror](https://github.com/MichMich/MagicMirror) project.

It shows the the menu including the prices of canteens from universities in germany and switzerland (based on openmensa.org).

## Screenshot
<img src="https://user-images.githubusercontent.com/9365668/69614485-7a552b80-1033-11ea-8885-54cd76336ca0.png"/>

## Installation
Clone the module into your MagicMirror module folder.
```
git clone https://github.com/k-0/MMM-Canteen.git

```

## Configuration
To display the module insert it in the config.js file. Here is an example:
```
{
    module: 'MMM-Canteen',
    position: 'bottom_center',
    config: {
        updateInterval: 10 * 60 * 1000,     // 10 minutes
        canteen: 63,                        // id from openmensa.org url [Example: https://openmensa.org/c/63] 
        status: "employees",                // choose between ["employees", "students", "pupils", "others"]
        truncate: 100,                      // truncate more than 100 letters                   
        switchTime: "16:00"                 // shows the menu from next day, if switchTime < now
}
}
```
