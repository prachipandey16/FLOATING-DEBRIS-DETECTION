# FLOATING-DEBRIS-DETECTION

# Abstract
Growing concerns about the environmental consequences of floating debris in aquatic ecosystems have underscored the need for the development of efficient and 
automated methods for debris classification and monitoring. This research paper presents a comprehensive investigation into the application of neural networks, specifically Convolutional 
Neural Networks (CNN), Long Short-Term Memory (LSTM), and CNNLSTM architectures, for this purpose. Our study entails the creation of a diverse dataset encompassing various 
debris types and environmental conditions, ensuring its realworld relevance and generalizability. Thorough exploration is 
conducted of the three neural network models to evaluate their effectiveness in classifying floating debris from images captured in aquatic environments. CNNs are chosen for their established 
image recognition capabilities, while LSTMs are incorporated to capture sequential information and potential temporal dependencies within debris trajectories. The outcomes of our 
study unveil the strengths and limitations of CNN, CNN-LSTM, and LSTM architectures in the context of floating debris classification. Proposed work provides insights into the 
suitability of each model in various real-world scenarios, including riverine systems, oceans, and coastal regions. Furthermore, we discuss the implications of our findings for 
environmental monitoring, debris removal strategies, and policy development. Throughout our research, each model's performance is assessed in terms of accuracy, precision, recall, 
and F1-score, considering the unique challenges posed by the inherently noisy and dynamic nature of aquatic environments. This research contributes to the evolving body of knowledge 
regarding the application of neural networks in environmental monitoring, with a particular focus on the critical domain of floating debris classification. Our findings are expected to guide 
the development of automated systems that can aid in mitigating the environmental impact of floating debris, ultimately promoting the sustainability of aquatic ecosystems

# Methodology
The approach for utilizing deep learning to address the challenge of floating debris in aquatic ecosystems encompasses a systematic
methodology that encompasses data collection, model development, and real-world application.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/8b16d98b-474f-4cee-9796-d5bc6620c38c)

The proposed framework to classify the floating debris is shown in Figure 1.

a) Dataset A study examined the spectral responses of common floating materials like seaweed, sea foam, and driftwood, as well as harmful substances such as sea snot and pumice, in comparison to plastic. The eighth Sentinel-2 spectral band revealed high reflectance for both driftwood and seaweed, allowing them to be easily distinguished from other materials. Driftwood showed a reflectance peak, while seaweed displayed an absorption peak, making them distinguishable from each other. Water had lower reflectance due to its high heat capacity. However, differentiating between plastic, pumice, sea snot, and sea foam based on spectral responses was challenging. To address this, spectral indices, which are mathematical equations combining values from multiple wavelengths, were employed to enhance the spectral features. The dataset [ ] included pixels from all floating materials, resulting in an imbalanced dataset with labels: 1 (water), 2 (plastic), 3 (driftwood), 4 (seaweed), 5 (pumice), 6 (sea snot), and 7 (sea foam).

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/7d457af5-d03e-483a-90b5-8df9e8525f2e)

The class imbalance issue within the dataset presented a significant challenge, where some classes were underrepresented compare to others. To mitigate this imbalance and enhance the performance of our machine learning models, we applied the Synthetic Minority Over-sampling Technique (SMOTE). SMOTE systematically generated synthetic samples for the minority classes, thereby rectifying the imbalance. The method strategically created artificial data points based on the characteristics of existing data, effectively increasing the number of instances in the underrepresented classes.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/3e1d5173-a674-4560-a328-c9d9a17471fd)

b) Preprocessing

One Hot encoding A(x):={1if x∈A,0if x∉A c) Deep Learning Techniques

CNN CNNs are specialized neural networks designed to recognize visual patterns in images. They achieve this through a mathematical operation known as convolution, which processes image data by multiplying matrices. CNNs consist of layers, including convolution and pooling, and employ a backpropagation algorithm to learn hierarchical patterns in data, enabling them to automatically recognize and categorize visual features in images.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/8fc1ed8b-6ef6-4f2b-a67c-f2315509ebe1)

LSTM LSTMs rely on a crucial element called the cell state, visualized as a horizontal line at the top of the diagram. Think of the cell state as a conveyor belt, smoothly transmitting information without significant alteration. However, LSTMs feature gates, which are composed of sigmoid neural net layers and pointwise multiplication operations. These gates allow for selective information flow, with values ranging between zero (blocking) and one (allowing passage). Typically, an LSTM has three gates that protect and regulate the cell state.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/864e765e-5f63-40c6-b1b8-295f8c95d024)

CNN-LSTM The CNN LSTM architecture is a robust blend of Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks. It excels in processing sequential data with both spatial and temporal dependencies, making it valuable in applications like video analysis, speech recognition, and natural language processing. This approach harnesses CNNs for feature extraction from spatial data and LSTMs for sequence modelling, widely employed in tasks requiring a comprehensive understanding of both spatial and temporal information to achieve precise predictions or classifications.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/de3ef6bb-2dc2-430a-b4ca-8c810a2d663d)

IV. RESULTS AND DISCUSSION The deep learning approach exhibited promising outcomes, underscoring the precision and consistency of Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks in the classification of aquatic debris. When integrated into real-time monitoring systems, this method delivers proactive surveillance and automated response capabilities, effectively tackling the global challenge of floating debris on a large scale. The models' capacity to adapt to varying environmental conditions and the amalgamation of data further bolster the methodology's resilience, establishing it as a groundbreaking approach with substantial implications for environmental preservation.

![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/d6c6475a-25b6-4928-a682-acf231b518f7)

1. CNN    ![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/d51d3252-4d8c-4aa7-9999-d3557dbf335e)
          ![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/ef95215b-7d92-46cb-8500-c5248033e79e)
2. LSTM   ![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/c71fd652-07fb-4ff2-8a23-2441b5e4b45d)
          ![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/e97ad74c-e80e-413b-80f9-5aae6007b875)
3. CNN-LSTM  ![image](https://github.com/prachipandey16/FLOATING-DEBRIS-DETECTION/assets/115707069/cbd31a73-5751-43a1-8d46-c08a9ba2e591)
             ![Uploading image.png…]()


REFERENCES [1] G. Eason, B. Noble, and I. N. Sneddon, “On certain integrals of Lipschitz-Hankel type involving products of Bessel functions,” Phil. Trans. Roy. Soc. London, vol. A247, pp. 529–551, April 1955. (references) [2] J. Clerk Maxwell, A Treatise on Electricity and Magnetism, 3rd ed., vol. 2. Oxford: Clarendon, 1892, pp.68–73. [3] I. S. Jacobs and C. P. Bean, “Fine particles, thin films and exchange anisotropy,” in Magnetism, vol. III, G. T. Rado and H. Suhl, Eds. New York: Academic, 1963, pp. 271–350. [4] K. Elissa, “Title of paper if known,” unpublished. [5] R. Nicole, “Title of paper with only first word capitalized,” J. Name Stand. Abbrev., in press. [6] Y. Yorozu, M. Hirano, K. Oka, and Y. Tagawa, “Electron spectroscopy studies on magneto-optical media and plastic substrate interface,” IEEE Transl. J. Magn. Japan, vol. 2, pp. 740–741, August 1987 [Digests 9th Annual Conf. Magnetics Japan, p. 301, 1982]. [7] M. Young, The Technical Writer’s Handbook. Mill Valley, CA:University Science, 1989.


