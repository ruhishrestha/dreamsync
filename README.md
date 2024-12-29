

# What is DreamSync?
Essentially, this device utilizes principles of electroencephalography (EEG) and transcranial electrical stimulation (TES) to create targeted low-intensity electrical pulses to basal ganglia pathways. By regulating these pathways, DreamSync seeks to:
- **Balance Circadian Rhythms:** Increases the communication between the basal ganglia and hypothalamic-pineal rhythms to regulate melatonin synthesis. 
- **Expedite Sleep:** Elevate melatonin levels naturally to improve sleep initiation. 
- **Advanced Sleep Quality:** Supports deeper sleep phases by optimizing hormonal balance. 
- **Provide Individualized Treatment:** Adjusts simulation patterns based on EEG feedback and neural activity.
  
<img src="IMG_FCC1AF6CCD25-1.jpeg" alt="Project Screenshot" width="800">

# Key Components of DreamSync

**Software Butterworth Bandpass Filter Algorithm:** Used to allow signals within a specific frequency range (0.5–47 Hz) to pass through with minimal signal distortion. 

**Breadboard:** A platform for connecting the prototype and components without soldering. 

**Jumper Cables:** Enable connections between components on the breadboard and to the Arduino for signal flow. 

**AD8232 ECG Sensor with 3-Channel Electrodes:** Amplifies and filters bioelectric signals from the body, making them suitable for processing. 

**Arduino Uno 3:** A microcontroller that processes the signals and sends data to a connected device for analysis. 

**ADS1115 Analog-to-Digital Converter:** Converts the analog signals from the AD8232 into digital form for precise data capture. 

## Future Implementations

**TL074 Amplifier with High (47 Hz) and Low (0.5 Hz) Band Filters:** Provides additional amplification and filtering for cleaner signal output. 

**TES & EEGNet AI Model Integration:** Processes EEG signal data through a convolutional neural network to analyze brainwave patterns.

# How does DreamSync function?

1. **Setup and Powering On:** Wear the DreamSync headband as seen on model and ensure all components (Arduino, ADS1115, AD8232, TL074) are properly connected to the breadboard and powered via a USB connection or battery.
2. **Signal Detection:** The electrodes capture faint electrical signals generated by neural activity in your brain. Signal Amplification and Filtering: The AD8232 module amplifies these signals and filters out noise, ensuring they are clear enough for further processing.
3. **Signal Conditioning:** The TL074 op-amp provides additional amplification and fine-tunes the signals for optimal quality. Analog-to-Digital Conversion: The processed analog signals are sent to the ADS1115, which converts them into precise digital data.
4. **Data Processing:** The Arduino receives the digital signals, applies algorithms (e.g., Butterworth bandpass filtering), and organizes the data for analysis. Data Analysis with AI: The processed EEG data is analyzed by the EEGNet AI model, which identifies patterns in brain activity, such as those associated with sleep states.
5. **Real-Time Feedback Loop:** The system continuously monitors brain signals and adjusts stimulation parameters to align with the user's current sleep-related brain state. Impact on the Brain: The tDCS stimulation encourages activity in neural circuits linked to sleep regulation, promoting deeper, more restful sleep by calming overactive regions and enhancing relaxation.

# The Science Inside Our Brains

DreamSync targets the brain’s basal ganglia, specifically in areas like the subthalamic nucleus (STN) and the globus pallidus internus (GPi), to influence the suprachiasmatic nucleus (SCN) contingently. 
The STN and GPi both have an important neurotransmitter that is connected to sleep: Gamma-aminobutyric acid (GABA).
GABA = an inhibitory neurotransmitter that slows down brain signals. This neurotransmitter then influences the SCN. 
SCN is a part of the hypothalamus that regulates the circadian rhythm by generating signals indicating the time of day. 
This will ultimately regulate the alkylamine N-acetyltransferase (ANNAT) activity within the pineal gland, promoting melatonin synthesis (a key hormone that regulates circadian rhythm). 
The ANNAT synthesizes melatonin by transferring an acetyl group to serotonin; this then creates  N-acetylserotonin. This then signals another enzyme called hydroxyindole-O-methyltransferase, which synthesizes N-acetylserotonin into melatonin.

<img src="IMG_7E25AC653C08-1.jpeg" alt="Project Screenshot" width="800">
