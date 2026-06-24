## 🤖 Model Information

The application uses a pretrained **NAFNet-GoPro-width64** model for motion deblurring.

| Property           | Value                                                                                               |
| ------------------ | --------------------------------------------------------------------------------------------------- |
| Architecture       | NAFNet (Nonlinear Activation Free Network)                                                          |
| Framework          | PyTorch                                                                                             |
| Parameters         | 29.16 Million                                                                                       |
| Dataset            | GoPro Large Dataset                                                                                 |
| Task               | Motion Deblurring                                                                                   |
| Paper              | [ECCV 2022](https://arxiv.org/abs/2204.04676)                                                       |
| Model Width        | 64                                                                                                  |
| Pretrained Weights | [nyanko7/nafnet-models](https://huggingface.co/nyanko7/nafnet-models) on Hugging Face Hub (~600 MB) |

### What is NAFNet?

NAFNet stands for **Nonlinear Activation Free Network**.

It is a deep learning architecture designed for image restoration tasks such as image deblurring, denoising, and super-resolution. Unlike traditional convolutional neural networks that rely on activation functions such as ReLU or GELU, NAFNet introduces non-linearity through a lightweight gating mechanism called **SimpleGate**.

This design improves computational efficiency while maintaining state-of-the-art image restoration performance.

Applications include:

* Motion Deblurring
* Image Denoising
* Image Super Resolution
* General Image Restoration

> **Note:** Model weights are downloaded automatically from Hugging Face Hub during the first inference request. Subsequent requests use the cached model for faster response times.

---

## 👨‍💻 My Contributions

This project was developed as an end-to-end AI application that integrates a pretrained deep learning model with a web-based user interface and cloud deployment.

### Frontend Development

* Designed and developed the complete user interface using HTML, CSS, and JavaScript
* Implemented drag-and-drop image upload functionality
* Developed image preview, side-by-side comparison, and image download features
* Connected the frontend to the backend through REST API calls
* Added user-friendly status messages and warmup notifications

### Backend Development

* Built the FastAPI inference backend and integrated the pretrained NAFNet model into a production-ready web application
* Implemented API endpoints for image upload, processing, and health checks
* Developed image preprocessing and postprocessing workflows
* Implemented lazy model loading to reduce startup time
* Built automatic model weight download and validation logic
* Added robust error handling and model-loading safeguards
* Implemented CORS support for frontend-backend communication

### Deployment & Integration

* Configured Docker deployment for Hugging Face Spaces
* Deployed and managed the backend API on Hugging Face Spaces
* Hosted the frontend using GitHub Pages
* Integrated frontend and backend into a complete working application
* Managed source code, version control, and deployment using Git and GitHub

### Model Usage

This project uses a pretrained NAFNet model for image deblurring. The NAFNet architecture (`NAFNet_arch.py`) and pretrained weights originate from the official NAFNet research implementation.

My contributions focus on application development, backend engineering, API design, frontend development, deployment, and end-to-end system integration built around the pretrained model.

---

## 📄 License

This project is licensed under the MIT License.

The NAFNet architecture (`NAFNet_arch.py`) is adapted from the official NAFNet implementation released under the MIT License by the original authors.

Original Repository: [megvii-research/NAFNet](https://github.com/megvii-research/NAFNet)

This repository additionally contains custom application code developed for:

* FastAPI backend development
* Image preprocessing and postprocessing pipelines
* API endpoint implementation
* Frontend development (HTML, CSS, JavaScript)
* Docker deployment configuration
* Hugging Face Spaces deployment
* GitHub Pages integration
* End-to-end application integration and deployment
