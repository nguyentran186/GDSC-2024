
# GDSC Hackathon VietNam 2024 (Poscify)

[![Firebase Firestore](https://img.shields.io/badge/Firebase-Firestore-blue?logo=firebase)](https://firebase.google.com/docs/firestore)
[![Firebase Authentication](https://img.shields.io/badge/Firebase-Authentication-orange?logo=firebase)](https://firebase.google.com/docs/auth)
[![MediaPipe](https://img.shields.io/badge/MediaPipe-Visit-blue?style=flat-square&logo=mediapipe)](https://mediapipe.dev/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-Explore-orange?style=flat-square&logo=tensorflow)](https://www.tensorflow.org/)
[![Kubeflow](https://img.shields.io/badge/Kubeflow-Discover-brightgreen?style=flat-square&logo=kubeflow)](https://www.kubeflow.org/)
[![Google Drive API](https://img.shields.io/badge/Google%20Drive%20API-Documentation-yellow?style=flat-square&logo=google-drive)](https://developers.google.com/drive)




<img align="right" width="180" alt="logo" src="https://github.com/hungmeomeo/poscify-mobile/assets/95847972/c59b1fa6-8696-4f81-9aba-a63fe891848e">

## About project
Poscify was born amidst the global threat of diseases related to eye and spine conditions caused by improper sitting habits. Poscify aims to improve posture and health for children, especially when they are sitting on school chairs, thereby enhancing societal awareness of education within families.
## Sustainable Development Goals of United Nations

<img align="right" width="100" alt="logo" src="https://github.com/hungmeomeo/poscify-mobile/assets/95847972/376699e3-3004-454b-9708-23fb77820f0f">
<img align="right" width="100" alt="logo" src="https://github.com/hungmeomeo/poscify-mobile/assets/95847972/8ab286ae-410f-4ebf-b501-e8edf581ff5a">




- Goal 3: Good Health and Well-being
Improving sitting posture contributes to a healthy foundation for children

- Goal 4: Quality Education 
Beyond analyzing posture, our solution emphasizes human values by involving parents in guiding posture correction for their children


## Video demo

https://drive.google.com/drive/folders/192E1hDc0UwuKMdJt3oqG_G-a5SgBtdmT







## Table of Contents
- [Technologies](#technologies)
- [Structure](#structure)
- [Installation](#installation)
- [Architecture](#architecture)
- [License](#license)

## Technologies 
This project was implemented using the following technologies:
- Mediapipe
- Tensorflow
- Firebase storage
- Firebase Google Auth
- Kuberflow
- Python 3
- React Native
- Google Cloud API, Go(Comming soon)


## Structure

```text
/
├── model
│   ├── api.py
│   ├── datacollect.py
│   ├── posture_data.py
│   ├── trainclassifer.py
│   ├── predict_demo.py
│   ├── predict_nofity.py
│   ├── model.sav
├── src
│   ├── assets
│   ├── components
│   ├── models
│   ├── pages
│   ├── utils
│   ├── App.js
│   ├── package.json
|   ├── README.md
│   ├── firebaseConfig.js
|   └── yarn.lock
```


## Installation
This project is designed to be run in Google Colab and Python IDE. After cloning the project, please follow these steps:

### For the `model` folder
1. Data Collection:

- Run python datacollect.py.
- Follow the prompts to adopt different postures and press the corresponding keys (B for 'okay', C for 'bad', D for 'terrible').
- Aim for 400 instances for each posture category.
- Press 'Q' to exit the program and save the collected data as posture_data.npy.
2. Model Training:

- Execute python trainclassifer.py to train the model. The trained model will be saved as model.sav.
3. API Setup:

- Launch the API by running python api.py.
- Once Flask has finished preparing, the frontend framework can interact with the API via socket on port 5000.
- Provide instructions on how to call the API in the README file.

### For the `app` folder
1. Clone the repository
2. Open the project in your preferred IDE (e.g. Android Studio, VS Code)
3. Run `npm install` to install the required dependencies
4. Run 'npm run android' or 'npm run ios' due to your preferences OS.
5. Run the project in an emulator or on a physical device

## Architecture
### Software architecture
![image](https://github.com/hungmeomeo/poscify-mobile/assets/95847972/895abed7-b0dd-485d-a025-50df60d6b629)
### Operation procedure
![image](https://github.com/hungmeomeo/poscify-mobile/assets/95847972/03284e75-cf01-48b4-8532-7a27e7d49be7)
### AI flow
![image](https://github.com/hungmeomeo/poscify-mobile/assets/95847972/6219dfaa-b0a5-4c09-b630-716ac4f204a2)



## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
