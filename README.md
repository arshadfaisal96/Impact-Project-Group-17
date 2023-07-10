# **Eselec - Generator Monitoring and Predictive Maintenance**
### Impact/Capstone Project - IE School of Science and technology - 2023

- Arshad Irfan Faisal
- Constança Salgado Corte-Real De Albuquerque
- Joao Ferris
- Yash Singh
- Zara Fatima Amer

----------------------------
### Overview
As we continue to advance technologically, the reliability, efficiency, and sustainability of our power generation systems grow increasingly
crucial. Central to these goals is the need for robust monitoring and anomaly detection within these systems. If undetected, anomalies or
irregularities in operational data can lead to inefficiencies, costly equipment damage, and even safety hazards. Addressing this issue is a
significant concern for ESELEC, a leading electrical machinery manufacturer, particularly within their power generator systems.
### The Problem
The primary challenge lies in detecting unusual patterns in the excitation current of ESELEC's generator systems. This aspect is critical as
improper regulation of the excitation current can cause severe problems, including equipment failure. Traditional anomaly detection methods,
while useful, often fall short in detecting subtle irregularities within the complex temporal nature of time series data.Traditional anomaly
detection methods have been employed in the past to identify irregularities in data. However, these methods often struggle to effectively detect
subtle irregularities within the complex temporal nature of time series data, such as the excitation current. The temporal nature of the data adds
an additional layer of complexity, as the patterns and trends may change over time, making it challenging to establish a fixed baseline for
anomaly detection.
### The Solution
To overcome this challenge, we proposed a solution leveraging advanced machine learning techniques, specifically Long Short-Term Memory
(LSTM) networks. LSTM networks, a type of recurrent neural network, excel in understanding time-dependent data, making them ideal for this
application. We used an LSTM-based autoencoder model that learns to compress the input data (time steps from our generator data) into a
lower-dimensional representation and then reconstructs the original data. If the data instance is normal, the autoencoder can reconstruct it
accurately. However, anomalies deviate from what the autoencoder considers "normal," resulting in a high reconstruction error which we use as
an anomaly score. This data-driven approach offers a robust understanding of the complex relationships in our multivariate time series
data.Furthermore, the data-driven nature of the solution provides a comprehensive understanding of the complex relationships within the
generator systems. This enables ESELEC to make informed decisions based on the anomaly scores and take necessary actions to rectify any
detected anomalies, ensuring the reliability, efficiency, and safety of their power generation processes. In summary, the proposed solution
leverages advanced machine learning techniques, particularly LSTM networks and the autoencoder model, to detect unusual patterns in the
excitation current. This data-driven approach empowers ESELEC to proactively identify and address anomalies, leading to improved operational
efficiency, reduced downtime, and substantial cost savings
### Impact
The implementation of this solution stands to benefit ESELEC significantly. By proactively detecting and rectifying operational deviations, the
company can substantially reduce operational costs, prevent machine breakdowns, extend the lifespan of machinery, and enhance safety. The
LSTM model was meticulously trained and validated to ensure reliability and accuracy in identifying operational deviations. The project's
success was gauged based on several critical indicators, including the accuracy of the machine learning model, the feasibility and efficacy of
derived recommendations, tangible improvements in machine efficiency, cost savings, and operational lifespan, and the reduction of safety
incidents.
### Future Work
While the results are promising, future work includes refining model hyperparameters, exploring other machine-learning techniques, expanding
the project scope to include additional machines, enhancing fault localization capabilities, and incorporating prognostics for predicting the
remaining useful life of generator components. These refinements contribute to increased operational efficiency, reduced downtime, and
improved overall performance of power generation units.
### Deployment
The system can be deployed in a cloud environment or locally, with a user-friendly interface for easier access and data exploration. We plan to
develop an interactive dashboard for users to explore data, with comprehensive user guidance and documentation provided. The model will need
regular monitoring and updates post-deployment to ensure its performance and relevance.
Overall, this project marks a significant stride towards operational optimization for ESELEC, promising long-term benefits that include
improved efficiency, heightened safety, and considerable cost savings. 
