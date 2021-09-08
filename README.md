# Singing Voice Separation in Musical Arrangements Using a Deep U-Net Convolutional Neural Network

The final project in the course **DT2119 Speech and Speaker Recognition** at KTH Royal Institute of Technology. The project focused on the task of separating the singing voice from the background arrangements in music. _STFT_- and _Log Mel Spectrum_-representations of musical data were fed into a modified _U-Net CNN_, and common metrics within the research field were utilized for evaluation. Data augmentations methods were analyzed and compared.

## Team Members

<ul>
    <li>
        <strong>Valdemar Gezelius</strong>
    </li>  
    <li>
        <strong>Lukas Frösslund</strong>
    </li>
</ul>

## Technologies

-   [Python3](https://www.python.org/)
-   [TensorFlow2](https://www.tensorflow.org/)
-   [Keras](https://keras.io/)
-   [SciPy](https://www.scipy.org/)
-   [Librosa](https://librosa.org/doc/latest/index.html)

## Project Details

The _MUSDB18_ dataset was used for this project. Preprocessing of the data included a transform to the frequency domain with an STFT, and conversion to the Log Mel Spectrum-representation. _Mel Frequency Cepstral Coefficients_ (MFCCs) were avoided due to the belief that our network could handle the feature correlation well, and that an additional DCT decorrelation process therefore was not necessary.

_Pitch Shifting_, _Time Stretching_ and _Random Amplitude Scaling_ were all used and compared as augmentations methods. The _binary cross-entropy loss_ was used as our loss function. As evaluation metrics, _SAR_ and _SDR_ was implemented.

More details available in the <a href="https://github.com/vgez/Deep-Learning-Singing-Voice-Separation/blob/main/Project_Report_DT2119.pdf">project report</a>.

## Visual Data Representation

![data_rep](https://github.com/vgez/Deep-Learning-Singing-Voice-Separation/blob/main/images/data_rep.png?raw=true)
