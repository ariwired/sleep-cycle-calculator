# Sleep Cycle Calculator

A minimalist mobile application built with Flutter to calculate optimal wake-up times based on the 90-minute sleep cycle rule. 

This project was developed as a practical study for a mobile development course, aiming to solve the problem of calculating sleep cycles quickly before bed without relying on web browsers or bloated alarm apps.

## How the math works

The average human sleep cycle lasts 90 minutes. Waking up in the middle of a cycle leaves you feeling groggy, while waking up at the end of a cycle makes you feel refreshed.

The app takes the base time, adds the dynamic fall-asleep delay (based on the selected tiredness flag), and then iteratively adds 90-minute blocks to generate the list of recommended wake-up times.

## Future Features

- **Cycle Calculation:** Calculates and displays all 6 sleep cycles (ranging from 1.5 hours to 9 hours of sleep).
- **Tiredness Flags:** Dynamically adjusts the time it takes to fall asleep based on your current state:
  * Exhausted (~5 mins to fall asleep)
  * Tired (~10 mins)
  * Normal (~15 mins)
  * Not sleepy (~30 mins)
- **Time Window Constraint:** Allows inputting your bedtime and a strict maximum wake-up time ("wake me up before X"). The app returns the best sleep cycles that fit within that specific time frame.
- **Visual Feedback:** Color-coded results to easily identify the ideal (5-6 cycles), acceptable (3-4 cycles), and poor (1-2 cycles) wake-up times at a glance.
- **Dark Mode First:** UI designed exclusively in dark mode with high contrast to prevent eye strain during nighttime use.

## Tech Stack

* Flutter
* Dart

## License

This project is open-source and available under the MIT License.
