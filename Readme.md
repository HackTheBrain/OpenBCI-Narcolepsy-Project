# OpenBCI Narcolepsy / BAT
BAT (Brain AssistanT) is there for you to provide predictive insight into epileptic and narcoleptic events. With our open API you will be able to connect to an ecosystem of apps and services that integrate with BAT to offer new, customized experiences. Version 1.0 of BAT was made my Team MobGem lab, 26th June 2016.

![image mockup](https://github.com/HackTheBrain/openbci-narcolepsy/blob/master/images/Schermafbeelding%202016-12-01%20om%2012.55.20%20a.m..png)

# Why
We were aiming to make a multimodal, integrative measurement tool of physiological signals that can have a wide application in today´s society. As part of this project we came up with the idea that, in case of an undiagnosed illness, physicians would preferably have as much data as possible that can help them make a correct diagnosis. Instead of restricting a person´s movement by letting them reside in a hospital bed, our aim was to make this entire process mobile.
Additionally, the idea was to integrate this into a wearable, which would disguise the measurement equipment and to prevent stigmatization due to your appearance.

Besides using physiological data for diagnosing patients, it could also help existing patients in increasing their safety and mobility in everyday life. The system could provide accurate, real time information that could be sent to relatives or emergency services in case of the detection of an emergency through the wearable device. Additionally, integration with other systems could be a realistic possibility. One example of this could be the integration of the system in cars that have an autopilot available, such as the Tesla Model S. This would be applicable to narcolepsy patients, but also to epilepsy patients, that can lose consciousness behind the wheel. The system will then register the loss ofconsciousness via the change in physiological signals and take over control and eventually steer the car to safety.

This device can be applicable to a broad target audience. There are an estimated 80.000 people in the Netherlands at any time that are in treatment for epilepsy (Wallace et al., 1998) and an estimated 30 new epilepsy patients per year on a population of 100.000 (Kotsoupolos et al., 2005). In case of one epileptic seizure, a person is restricted from driving for three to six months. In case of two seizure events within a one year period, a person is restricted from driving for the period of one year (Cbr.nl, 2016). In case of narcolepsy, there are an estimated 20-50 people suffering from narcolepsy on a population of 100.000 (Ahmed & Thorpy, 2010). In the United Kingdom, people with narcolepsy can be allowed to drive after assessment of their condition by the Driver and Vehicle Licensing Agency (DVLA). They will be given a license for a short period of time if their condition is assessed to not endanger themselves or other road users. However, in the event that they do suffer from a narcolepsy attack our wearable device can be a literal life safer.

The wearable that we are planning to use is a cap integrated with electrodes, to measure alpha waves (8-12 Hz) from the occipital lobe, as has been used before by Tsai et al. (2009) to measure drowsiness in drivers. Alpha waves registered from EEG equipment are associated with concentration and BAT, your digital brain assistant 3 relaxation and in case a person closes his/her eyes, it shows a peak in the alpha spectrum.

![cap](https://github.com/HackTheBrain/openbci-narcolepsy/blob/master/images/Schermafbeelding%202016-12-01%20om%2012.50.02%20a.m..png)

Additionally, muscle tension has been shown to decrease during sleep. Our device will also have an EMG capability to measure the muscle tension of the patient and to ensure that, in case of loss of this muscle tension, a signal is being sent to the device and appropriate action can be taken.

WHAT
What are we creating?
BAT (Brain AssistanT) is there for you to provide predictive insight into epileptic
and narcoleptic events. With our open API you will be able to connect to an
ecosystem of apps and services that integrate with BAT to offer new, customized
experiences.
BAT will look into measuring the following channels:

- Alpha Waves
- Muscle Tension
- Heart Rate

When signals of an epileptic or narcoleptic event are being detected, BAT will
send out a notification towards the user. The notification will be linked towards
an action, which is related to the interface of the user.
Those signals, translated into actionable and meaningful information can be
used to inform and, most important of all, protect the user and it's surroundings.
But how can we translate data to meaningful information?


## What
*What are we Creating?* BAT (Brain AssistanT) is there for you to provide predictive insight into epileptic and narcoleptic events. With our open API you will be able to connect to an ecosystem of apps and services that integrate with BAT to offer new, customized experiences.

BAT will look into measuring the following channels:

- Alpha Waves
- Muscle Tension
- Heart Rate

When signals of an epileptic or narcoleptic event are being detected, BAT will send out a notification towards the user. The notification will be linked towards an action, which is related to the interface of the user.
Those signals, translated into actionable and meaningful information can be used to inform and, most important of all, protect the user and it's surroundings. 

*But how can we translate data to meaningful information?*
Our goal is to make “scientific data” meaningful and useful for everyone. Providing visualisations to the patients is useful, but we want to take it even further and provide simple functionality and user-friendly interfaces. Furthermore, we want to keep the element of fun to not make patients feel even worse by confronting their own defects. Providing different levels of overview will give the users the option to handle their own data with as much detail they wish.

Indicative functionality/Example scenarios:

- When the user is driving and is unfortunate to have unusual brain signals (to a threshold of an attack that could threaten their lives or render them impossible to continue driving), then an equipped car (Tesla) could take over and safely stop/park the car.
- ICE contacts or first respondents can be quickly notified about events and their severity. Imagine that when the system tracks an anomaly, that activity can be compared to the aggregated data of the specific user. In that way it can determine the severity, e.g. comparing to the average “attack duration” the user usually has. Based on the severity it can take drastic measures (e.g. send an SMS to the doctor), or just inform selected people on the incident via a chat bot.
- The user themselves can get all kinds of events monitored and classified, in zero time. Observing those data can bring more awareness, and perhaps understanding of their uniqueness due to the patterns that the app can track down (e.g. is there a time of the year that associates with more “brain” crises?). They can already offer their doctors a 24/7 report (if they wish to).

Example interfaces are:

- Tesla in-car display
- Smartphone
- Conversational interfaces (e.g. Facebook Messenger bot)

## Additional information on processing data with BAT:

- Store the sample next to the previous ones (cache)
- Filter out the noise (7-13hz, bandpass)
- Compare the sample from the previous ones
- Calculate if the last couple samples exceed a threshold
- Notify the user (in case it's falling asleep)

## References
Ahmed, I. and Thorpy, M. (2010). Clinical Features, Diagnosis and Treatment of Narcolepsy. Clinics in Chest Medicine, 31(2), pp.371-381. Cbr.nl. (2016). CBR | epilepsie. [online] Available at: https://www.cbr.nl/11468.pp? [Accessed 26 Jun. 2016].

Narcolepsy.org.uk. (2016). Narcolepsy and driving | Narcolepsy UK. [online] Available at: http://www.narcolepsy.org.uk/resources/narcolepsy-and-driving [Accessed 26 Jun. 2016].

Kotsopoulos I, Krom M de, Kessels F, Lodder J, Troost J, Twellaar M, et al.Incidence of epilepsy and predictive factors of epileptic and non-epileptic seizures. Seizure, 2005; 14(3): 175-182.

Tsai, Pai-Yuan, et al. "A portable device for real time drowsiness detection using novel active dry electrode system." 2009 Annual International Conference of the IEEE Engineering in Medicine and Biology Society. IEEE, 2009.

Wallace H, Shorvon S, Tallis R.Age-specific incidence and prevalence rates of treated epilepsy in an unselected population of 2,052,922 and age-specific fertility rates of women with epilepsy [see comments]. Lancet, 1998; 352(9145):
1970-1973.
