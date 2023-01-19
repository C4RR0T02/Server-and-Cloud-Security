# Artificial Intelligence for Cybersecurity

## Demystifying Artificial Intelligence for Security

### What is Artificial Intelligence

#### Natural Intelligence

        - Acquire and store knowledge
        - Reason based on stored knowledge
        - Able to take cues from environment
        - Make rational decisions based on collective learning for complex and conflicting situations

#### Artificial Intelligence

        Intelligence demonstrated by machines

#### Intelligent Agent

        - Machine, software or system
        - Maximize the probability of goal completion
        - Sensing, Learning, and acting

#### Digital Transformation

        - Digitalization of Personal Information
        - Cloud Migration
        - Internet of Things
        - Increase of data to protect

### Artificial Intelligence for Security

Intelligence Agent sifts through massive amount of data and learns
    - Identify patterns that are normal and expected 

#### When placed in the line of defense
1. Analyze incoming data
2. Uncover data patterns that are extremely difficult to analyze
3. Classify or categorizes the data 
4. Present pattern to security professional to assist in analysis

#### 3 Types of Artificial Intelligent Agents
1. Predictive Insights
2. Actionable Recommendation
    - Makes recommendations to the security professional on what actions to take
3. Autonomous Mitigation
    - Takes corrective action on behalf of security professional to mitigate the security issue

#### AI Augments current Environment
- People
- Processes
- Tools

#### AI at Continuum of Security
1. Prevention
    - Scan Source code and components
    - Threat modeling
2. Detection
    - Malware
    - Network and endpoint intrusion
    - User behavior
3. Response
    - Context
    - Security Operations
    - Automatic migration

### Foundation Disciplines of AI

#### 6 Foundational Capabilities
1. Understand Natural language
2. Store Information
3. Reason
4. Learn from new information
5. "See" and perceive surrounding objects
6. Manipulate and move physical objects

        Not all disciplines are required for an Intelligence Agent

#### Minimum Traits of AI Security Systems
1. Large Data
    - Process and learn from (train on) large volumes of data
2. Patterns and Relationships
    - Identify Patterns in or relationship among data
3. Adapt
    - Adapt to changes in environments by incorporating new data signals
4. Action
    - Makes recommendation, prediction or even take autonomous corrective action

### Discipline of Learning

#### Learning by Training

- Not Preprogrammed
- Trained the system to identify program execution patterns

#### Paradigm of Traditional programming

- Software Engineer identifies all possible inputs and conditions that a software will be subjected to
- Creates a software program that is able to handle those and only those input conditions
- Fail to handle that situation if not designed

#### Paradigm of Learning in Artificial Intelligence

- Data Science Team first identifies training data
    - Source code
    - log files
    - Program execution context.
- Feed the data to machine learning models
- Best fit model ready to act on new incoming data not previously seen

## Security Objectives and Approaches

### End-to-End Security Framework

#### CIA Model
- Confidentiality
- Integrity
- Availability

#### Orchestrated Framework
- Prevention
- Detection
- Response
- Feedback

        `Requires Qualified Security Professional`

### Problem of Shortage of Qualified Security Professionals
1. Gap in the Organization's ability to prevent and respond to threats
2. Burden on existing information Security Professional
    - Human Fatigue
    - Job dissatisfaction
    - Stress
    - Depression

### Solution for Shortage of Qualified Security Professionals

1. Workforce Development
2. Security by Design
3. Security Automation
4. Artificial Intelligence

### Security Controls

Prevent a security incident by applying layers of `administrative`, `technical`, and `physical` controls

#### Prevention Controls

1. Culture of security: Shared responsibility and training
2. Security policies, standards and processes
3. Hiring and screening
4. Identify and access management
5. Secure development lifecycle

#### Detection Controls

1. Intrusion Detection
2. Monitor data and configuration integrity
3. Malware detection
4. Social engineering attacks detection
5. SOC (Security Operations Center) and SIEM (Security Information and Event Management)

#### Response and Feedback Controls

1. Alerts
2. Meaningful context for triage and decision
3. containment and spillover minimization
4. Lesson Learnt

#### Characteristics of Security Problems
1. Problem of Scale
2. Problem of Context
3. Problem of Precision and Accuracy
4. Problem of Speed

## Leveraging AI to Solve Complex Security Problems

### Problems of Scale

#### Scale Challenge with Big Data

- Complex Data
- Security Tools
- Failure to Scale

#### Intrusion Detection System

##### Types of IDS

1. Network Intrusion Detection System that 
    - Monitors the traffic pattern for entire network activity
2. Host Intrusion Detection System 
    - Monitors a particular machine

##### Purpose of IDS

- Constantly scan and parses network packets and logs data
- Looks for signatures by pattern matching approach
    - Known malicious pattern in packet flow or binary code

##### Types of Data required to sift through

- Source of data
    - Network Layer Packets
    - Ethernet Frames
    - Web Server Logs
    - Application Logs
    - File Header and Contents
- Variety of attributes / Features
    - Protocol
    - IP (Destination / Source)
    - Contains_Script
    - Time of Day
    - Num_Special_Chars
    - Previous_state

##### Training and Deploying the Model

1. Train the Predictor Model
2. Deploy the Model
3. Detect Intrusion

### Problem of Context

#### Data Loss Prevention (DLP)

- Confidential data crossing trust boundary
- Text matching approach
- Tough problem to get right

#### BUilding Context with AI

- Training Set
    - Protected Words
        - Words and Phrases to be protected
    - Unprotected Words
        - Words and Phrases to be ignored
    - Semantic Relationships
        - Word embedding 
- Trained using different Learning Algorithm
- Able to recognize relationship (Spacial distance) between the words
- Sensitivity Level assigned to the document

### Problem of Precision and Accuracy

#### Dangers of False Alarms

##### Acting on false alarms  

    1. Waste organizational resources
    2. Distracts team from real issues

#### False Positive and Negatives

False Positive
- Treat genuine website as a fraud

False Negative
- Fail to detect fraud website

#### Features Selection for phishing detection

1. Reputation
    - TLS Certificate
    - Incoming Links
    - Outgoing Links
    - Alexa Rank
    - Whois Records
2. Network
    - Ping, TTL 
    - Protocol
    - Hosting Server
    - Server OS
    - DNS Records
3. Content
    - Domain Name
    - URL
    - Home Page
    - Child Pages

### Problem of Speed

- Companies required to `Act Fast`
- Attackers are `Stealthy` 
- AI able to `catch`

#### Speed with Predictive Analytics

- AI prepares you to be one step ahead of the adversary
- Giving the ability to predict the likelihood of future incidences

#### Predicting Risky Authentications

- Behavioral Characteristics
    - IP Address
    - Service Accounts VS User accounts
    - Frequency of auth requests
    - Country, City
    - Day and time of day
    - Device footprint
    - Simultaneous multi-region sessions
    - Previous login attempts

## Machine Learning for Security

### Categories of Machine Learning

#### Commonly Interchanged Terms

`Discipline of Learning` is one of the **capabilities** of `Artificial Intelligence` 

`Machine Learning` is a **type of learning** that uses statistical techniques and modeling to perform a task without programming

`Deep Learning` is a **type of machine learning** that uses layering of many algorithms

`Deep Learning` tries to mimic the ways neural networks in our brain function

#### Choice of Machine Learning Algorithms

- Factors influencing selection of machine learning algorithms
    - Type of training data
    - Type of Problem

##### Type of training data

|Labeled|Unlabeled|
|--|--|
|`Prior knowledge` of relationship between data and desired outcome|`No Prior Knowledge` of relationship between data and desired outcome|
|`Supervised` Learning|`Unsupervised` Learning|

##### Type of Problem

1. Predict a future event from past data
    - Regression
2. Split data into known categories
    - Classification
3. Discover new patterns in data
    - Clustering
4. Generate synthetic data
    - Generative

### Prediction by Regression

Regression attempts to build a mapping function between the input variables and the output variables

#### Regression Problems 

- Number of tampered IoT devices
- Intensity: Number of packets sent per second (Dos/ DDos)
- Impact: Number of compromised machines

#### Regression Algorithms

- Linear Regression
    - Algorithm generates a model that is as simple as a linear equation between the input and output variable
- Support Vector Regression
    - Allow you to build more complex models around a curve rather than a straight line
- Random Forest
- Decision Trees
- Regression ANN (Artificial Neural Network)

### Classification of Good VS Bad

Classification is the process of segregating new data into previously known categories

#### Regression VS Classification

|Regression|Classification|
|--|--|
|Output of the model is a `numeric variable`|Output a `categorical variable`|
|Solve a problem such as `predicting the number` of XXX|`Determine` whether the XXX contains XXX|

#### Solving Classification Problems

Choose classified algorithms that map data into categories
- Logistic Regression
- K-near neighbors (KNN)
- Support Vector Machines (SVM)
- Naive Bayes
- Decision Tree Classification
- Random Forest Classification
- Classification ANN (Artificial Neural Networks)

### Clustering, Pattern, and Anomaly Detection

Clustering algorithms group or cluster data with similar characteristics together

#### Classification VS Clustering

|Classification|Clustering|
|--|--|
|Categories are `previously known`|`No pre-conceived notion` about the groups|
|Supplied via `labeled training data`|Creates the groups without any oversight (`No Labels`)|
|`Supervised` learning|`Unsupervised` learning|

#### Clustering Use Cases

1. Pattern Recognition
    - K-means
    - Self Organizing Maps
2. Anomaly Detection
    - DBSCAN (Density-based spatial clustering of applications with noise)
    - Bayesion Gaussian mixture models

### Synthetic Data Generation

Generate new data that follow the same probability distribution function

#### Synthetic Data Use Cases

- Cracking Passwords
- Fuzz Testing
- Vulnerability Testing
- Steganography

#### Why Synthetic Data Generation?

- Statistical model will not be able to distinguish between the new and the old data
- Do not want to provide original set of data
- Still share a representative sample with someone for testing

#### Synthetic Data Generation Algorithms

- Markov Chains
- Boltzmann machines
- GANs (Generative adversarial networks)

#### Deepfakes using GANs

- Replace the person's face with the face of another

## Practical Considerations, Risks, and Limitations

### Three Ways AI can Fail You

1. Limitations and Poor Implementation of AI
2. Attacks Against Your AI Implementation
3. Use of AI By Criminals

### One: Limitations and Poor Implementations

1. Machine Learning is Probabilistic
    - No domain knowledge
    - Add constraints to algorithms
2. Lack of explainability
    - Cannot explain intuitively the rationale behind its decision
    - No supporting explanation when presented with a recommendation or action
3. Insufficient Dependencies
    - Require large volume of training data
    - Labeled Data

#### Probabilistic system

Determines the probability of occurrence of an event

#### Issues of Probabilistic system

1. There is always going to be a `degree of error` associated with the `probability`
    - Model Error
    - Bias Variance
    - Auto Correlation
2. `False Positives` and `False Negatives` with the `recommendation` made by your AI system

### Two: Attacks Against Your AI Implementation

#### Breed of attacks

AI is vulnerable to attacks

Exposure to: 
1. New attack surface
2. New ways of Exploitation

#### Attack on Confidentiality

Attacks against the `confidentiality` of your AI system aim to `uncover` the `details` of the `algorithms` being used.

##### Inference Attack
- AI system aim to uncover the details of the algorithms being used
- Information used to plan for more targeted attacks

##### Timing of Attacks

- During Model Training
    - Attack on the Algorithm
- During Production
    - Attack on the Model

##### Things that can be inferred

- Training Data
- Attributes
- Algorithm

#### Attack on Integrity

Attacks on the `integrity` of your AI system aimed to `alter` the `trustworthiness` of its `capability for the task` it is designed to perform.

##### Timing of Attacks

- During Model Training or Feedback Loop
    - Data Poisoning
    - Adversarial or mutated inputs
- During Production
    - Adversarial or mutated inputs

##### Adversarial or mutated inputs

- Data input that `looks valid` but is `invalid`
- `Fools` the classifier such that the same data input belongs to the other classifier group

#### Data Poisoning

- Models behavior is modified
- Model is skewed on successful attack
- `Permanent` unless `model is trained again` with a `clean` and `trustworthy` training data

#### Attack on Availability

- Take control of model using `adversarial reprogramming`
    - Attacker `takes control of the model` and makes the model `perform a completely different task` than it was designed to perform
- Exceed computational and memory resources

### Three: Use of AI By Criminals

#### AI in an Attacker's Toolbox

- Attack with `Minimal Manual Effort`
    - Tasks requiring creativity and human intelligence remain manual
    - Captcha
    - Full undetectable (FUD) malware
        - VirusTotal
- Attack with `Precision and Accuracy`
    - Help with tracking targeted individuals social media, recent travel and other online or offline footprints
    - Operationalizes the Machine Learning model to automatically build and perform a task
- Attack `without Attribution`
    - Non-repudiation
    - AI introduce another degree of separation
- Attack with `Audio Video Manipulation`
    - Malicious use of deepfakes

### Getting Your Organization Ready for AI

Six Guiding Principles `do not replace` your current organizational framework. Rather, they `supplement` so you can do the due diligence and `set the realistic expectations` with your AI projects

#### Six Guiding Principles

1. Data Readiness
2. Experimentation
3. Core Competency
4. Measurement
5. Feedback Loops
6. Education

##### Plan for Data Readiness

- Data lives in Silos and under many custodians
- Data can be messy, inconsistent, and inaccurate
- Take data inventory
- Access to data by models during training and deployment

##### Embrace Experimentation

- You may not get it right the first time
- No plug-and-play or turnkey solution
- Pick one use and demonstrate value
- Learn from mistakes and iterate

##### Access your Core Competency

- Evaluate your skill-set, resources and willingness
- Choose a go-forward option
    - Hybrid
    - Buy
    - Build

##### Plan to Measure

- No guarantee, AI will perform better
- Develop and implement a measurement framework
- Report ROI on AI investment
- Showcase improvement over status quo

##### Plan for Feedback Loops

- New threats emerge
- Models make mistakes
- Feed model performance data back into model for relearning

##### Plan for Education and Awareness

- Educate Security teams
- Make them excited about outcomes
- Explain to the staff how an AI approach can help them grow and be more effective

### Evaluating AI-based Products

#### Dimensions of Capability Evaluation

##### Model Training

1. How often they are trained, and by whom?
2. Who will provide the training data? 
3. What about the data from your environment? 
4. Who will train the model? 
5. Ask the vendor about the alternatives if label data is not available.
6. What capabilities does their product have for applying unsupervised learning?
7. How does the vendor handle and implement feedback loops?

##### Product Integration

Capability to
- Integrate vendor product into your unique environment
- Build instrumentation for measurement
    - Draw meaningful metrics in the entire data pipeline, from training, testing, and post-deployment
- Automatically orchestrate training and deployment models

##### Proof of Concept

- Time taken from install to first actionable insight
- Eagerness to do a proof of concept with your data

##### Native or Bolt-On AI

- Developed In-house or Acquired?
- All Integrated from ground up or just another "Insights" module

##### Security and Privacy of Data

- Who owns the data?
- Any data reported back to vendor?
- Protection from data poisoning, adversarial, and evasion attacks
