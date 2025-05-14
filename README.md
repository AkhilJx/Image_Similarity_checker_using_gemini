# Image Similarity Checker with Gemini 1.5 Pro

A Streamlit web application that compares two images using Google's Gemini 1.5 Pro model, providing a similarity score and detailed justification for the result.

## Features

- **Dual Image Upload**: Upload two images for comparison
- **File Type Validation**: Ensures only image files are uploaded
- **AI-Powered Analysis**: Uses Gemini 1.5 Pro for intelligent image comparison
- **Detailed Results**: Provides both a similarity score (0-100%) and a textual justification
- **User-Friendly Interface**: Clean, intuitive UI built with Streamlit

## How It Works

1. User uploads two images via the Streamlit interface
2. System verifies both files are valid images (JPG, PNG, etc.)
3. Valid images are sent to Gemini 1.5 Pro for analysis
4. AI model compares the images and generates:
   - A similarity score (percentage)
   - A detailed explanation of the comparison
5. Results are displayed to the user in a clean format

## Supported Image Formats

- JPEG/JPG
- PNG
- Many other formats can also be included if needed, like WEBP, GIF (first frame will be used), BMP etc 

## Implementation

streamlit run app.py
Open your browser to the provided local address (typically http://localhost:8501)
Upload two images using the file uploaders
View your similarity results!

## Example Output

Similarity Score: 85%

Justification:
The two images show very similar compositions with the same subjects in nearly identical positions. 
The color palette and lighting are virtually the same, though there are minor differences in 
the background details. The main subjects match about 90% of features, while the backgrounds 
show about 80% similarity due to some variations in peripheral objects.

![image](https://github.com/user-attachments/assets/b0104bc8-c22d-4fa2-a514-e21b556c8d2d)


## Requirements

Python 3.8+

Streamlit

Google Generative AI SDK

python-dotenv

Pillow (for image processing)

## Limitations

Large images may take longer to process

Very dissimilar images may receive generic justifications

Abstract art/complex images may not compare as accurately

## Future Possibilities

Can make use of face detection tools like Huggingface models or Google Mediapipe library to verify that the user uploaded image has a face in it.
 
