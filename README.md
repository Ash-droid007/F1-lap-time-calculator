# F1-lap-time-calculator
A simple c program that calculates lap time based on car speed and track length. My first step in combining F1 with coding.
📌 Features
* Takes track length (in km) as input.
* Tkaes car speed (in km/h) as input.
* Calculates lap time in seconds.

```c
#include <stdio.h>

int main() {
    float track_length, car_speed, lap_time;
    printf("Enter track lenth (in km): ");
    scanf("%f", &track_length);
    
    printf("Enter car speed (in km/h): ");
    scanf("%f", &car_speed);
    
    float speed_km_per_s = car_speed/3600.0;
    
    lap_time = track_length/speed_km_per_s;
    
    printf("At %.2f km/h, the car completes %.2f km track in %.2f seconds.", car_speed, track_length, lap_time);


    return 0;
} 
```

Example Output 
```
Enter track lenth (in km): 200
Enter car speed (in km/h): 40
At 40.00 km/h, the car completes 200.00 km track in 18000.00 seconds.
```

🎯Future Plans
* Add support for multiple laps.
* Compare two cars on the same track.
* Store result in a CSV file for analysis.

