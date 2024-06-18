# PPG_Signal_Dataset

This repository contains a collection of 2-minutes resting-state photoplethysmography (PPG) signals from 59 subjects of both sexes (40% female and 60% male) with ages ranging from 15 to 85 years. Along with the PPG signals, we provide some information about the participants' habits and observations that might affect the signal quality.


## Device 

The acquisition module consisted of a sensing and a digitization module. 

The sensing module was a Mindray reusable fingertip SpO2 sensor, model 512F-30-28263. According to the manufacturer, the best monitoring location is the index finger, although other fingers can be used if the index finger is not available or the signal cannot be acquired correctly. 

<img width="299" alt="Captura de Pantalla 2024-06-17 a la(s) 20 04 24" src="https://github.com/lucilacapurro/PPG_Signal_Database/assets/95888088/e4bbc7c6-a587-4258-826f-a9ed3ca20dd9">

<img width="276" alt="Captura de Pantalla 2024-06-17 a la(s) 20 04 11" src="https://github.com/lucilacapurro/PPG_Signal_Database/assets/95888088/c5f9cef3-0397-4115-a71c-67d476b4257e">


Analog data from the sensor was sent to the digitization module via a DB9 connector for digitization using the ADC. The digitization module consisted of the AFE4490SPO2EVM board from Texas Instrument.

<img width="388" alt="Captura de Pantalla 2024-06-17 a la(s) 20 03 31" src="https://github.com/lucilacapurro/PPG_Signal_Database/assets/95888088/422592b5-e1e9-43c8-a9f3-e62160d04e13">

Then, the board communicated with the central module (PC) via a mini-USB to USB-A cable. Communication was carried out using the protocol provided by Texas Instruments, so the digitized signal was sent to the PC for storage and further processing.

The PPG signal was sampled at 500 Hz and stored in a CSV file.


## Signal acquisition protocol

The volunteers had the sensor placed on their index finger (or thumb for very small index fingers) and were asked to remain relaxed for 2 minutes while their PPG signal was acquired. The patient's finger was placed over the sensor's monitoring window with the fingertip against the stop, ensuring that all the light emitted by the sensor passed through the tissues. The patient was asked to remain still and quiet to ensure accurate readings.
Additionally, they were asked about their sex, age, if they had any known heart diseases, and if they regularly exercised or smoked.


## Participant Information

- Sex Distribution: 40% Female, 60% Male
- Age Range: 15 to 85 years

<img width="727" alt="Captura de Pantalla 2024-06-17 a la(s) 20 10 27" src="https://github.com/lucilacapurro/PPG_Signal_Database/assets/95888088/faab3378-d02f-4a02-a213-3962213538cc">

- Heart rate distribution:

<img width="616" alt="Captura de Pantalla 2024-06-17 a la(s) 20 08 10" src="https://github.com/lucilacapurro/PPG_Signal_Database/assets/95888088/c59f888b-4de5-4c5c-b44b-0e66b70f5090">

- Habitual Information:
    - 53% exercised regularly
    - 3% were regular smokers
    - 3% both exercised and smoked regularly
- Observations:
    - 5 subjects had painted nails
    - 1 subject reported having a pacemaker
    - 1 subject had a known heart disease
    - 1 subject experienced hand tremors on the hand where the sensor was placed

