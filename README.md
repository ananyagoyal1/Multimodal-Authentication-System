# Multimodal Authentication System

This project implements a multi-step authentication system that combines facial recognition, a real-time task, and a CAPTCHA verification process. The system is designed to enhance security by requiring users to pass through multiple authentication layers before gaining access.

## Features

- **Facial Recognition**: The system uses OpenCV to detect and recognize faces from the camera feed. It compares the captured face image with stored biometric data to verify the user's identity.

- **Real-time Task**: After successful facial recognition, the user is prompted to complete a real-time task. This task involves typing a randomly generated number within a specified time frame, ensuring that the user is present and actively engaging with the system.

- **CAPTCHA Verification**: Upon completing the real-time task, the system generates a CAPTCHA based on the task result. The user must correctly enter the last digit of the CAPTCHA to confirm their identity and complete the authentication process.

## Prerequisites

Before running the Multimodal Authentication System, ensure that you have the following dependencies installed:

- Python 3.x
- OpenCV (cv2)
- NumPy

You can install the required Python packages using pip:

```
pip install opencv-python numpy
```

## Usage

1. Clone the repository to your local machine:

```
git clone https://github.com/your-username/multimodal-authentication-system.git
```

2. Navigate to the project directory:

```
cd multimodal-authentication-system
```

3. Run the `main.py` script:

```
python main.py
```

4. Follow the prompts in the terminal:
   - Enter your username when prompted.
   - Look at the camera for facial recognition.
   - Complete the real-time task by typing the displayed number.
   - Enter the last digit of the CAPTCHA based on the task result.

5. If all authentication steps are successful, the system will grant access. Otherwise, it will deny access and terminate the authentication process.

## Customization

The Multimodal Authentication System can be customized and extended to meet specific requirements. Here are a few potential modifications:

- **Facial Recognition Model**: Replace the pre-trained face detection model with a more advanced or custom-trained model for improved accuracy.
- **Real-time Task Complexity**: Increase the complexity of the real-time task by introducing different types of challenges, such as puzzles or arithmetic operations.
- **CAPTCHA Generation**: Enhance the CAPTCHA generation process to create more complex and secure CAPTCHAs, e.g., using images or audio challenges.
- **Database Integration**: Integrate the system with a database to store and manage user biometric data and authentication records.
- **Logging and Reporting**: Implement logging and reporting mechanisms to track authentication attempts, successes, and failures for auditing purposes.

## Contributing

Contributions to the Multimodal Authentication System are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- OpenCV for providing the computer vision library used in facial recognition.
- NumPy for numerical computing support.
