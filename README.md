## README




### 1.Project Title: Photorealistic Hand Avatar Texturing with Palmar and Dorsal Hand Views
https://github.com/Meghnashankr23/3DVSS_June2026/blob/main/Photorealistic_Hand_Texture.ipynb
<img width="579" height="421" alt="UV texture" src="https://github.com/user-attachments/assets/de732f24-9a12-445e-97c9-913d2a6b49cf" />
Texture outputs given the Palmar and Dorsal Images of subjects

### Overview
This Colab notebook demonstrates a novel and efficient approach for generating photorealistic textures for 3D hand models. It specifically addresses the challenges of accurately representing both the palmar (front) and dorsal (back) sides of the hand by leveraging a ControlNet-based texture generation pipeline conditioned on anatomical priors.

The notebook covers:
-   **Environment Setup**: Installation of necessary libraries (`diffusers`, `ip-adapter`, `opencv-python`, `pyvista`, etc.) and downloading project assets (`Demo.zip`).
-   **Input Preparation**: Loading and displaying control images (UV normal, depth, mask) and semantic UV maps, along with reference images for the back and palm of the hand.
-   **Semantic Masking**: Creating semantic masks for distinct hand regions (palm and back) to guide the diffusion process.
-   **Model Configuration**: Loading pre-trained ControlNet models (for normal and depth guidance) and configuring the IP-Adapter for style conditioning.
-   **Texture Generation**: Running the diffusion process separately for the back and palm of the hand, applying masks and specific prompts to generate region-specific textures.
-   **Texture Compositing**: Merging the generated back and palm textures based on semantic masks to create a final, cohesive UV albedo texture.
-   **Visualization**: Displaying the generated UV texture and applying it to a 3D hand mesh (`MANO_UV_right.obj`) for interactive visualization using `pyvista`.

This method enables rapid creation of personalized photorealistic hand avatars for various applications like XR, gaming, telepresence, and digital humans, generating high-quality UV texture maps in under one minute from minimal input.


### 2.Project Title: SMPLX Model Visualization and Animation
https://github.com/Meghnashankr23/3DVSS_June2026/blob/main/SMPLX_Animate.ipynb
<img width="1013" height="565" alt="image" src="https://github.com/user-attachments/assets/d12ca9df-1112-444f-b2a9-7a909df2b529" />
Image Source: https://github.com/facebookresearch/frankmocap/issues/91
### Overview
This Colab notebook demonstrates the loading, manipulation, visualization, and animation of the SMPLX human body model. It uses Python libraries such as `smplx` for model functionality, `trimesh` for 3D mesh processing, and `plotly` for interactive 3D visualizations and animations.

The notebook covers:
-   **Environment Setup**: Installation of necessary libraries (`smplx`, `trimesh`, `gdown`, `plotly`, `imageio`).
-   **Model Loading**: Downloading and initializing the SMPLX model files.
-   **Model Inspection**: Verifying model output dimensions (vertices and joints).
-   **Body Manipulation**: Adjusting body shape (`betas`) and pose (`body_pose`) parameters.
-   **Visualization**: Static and interactive 3D rendering of the SMPLX mesh and its joints using `trimesh` and `plotly`.
-   **Animation**: Creating dynamic animations of pose variations and custom pose sequences.



### How to Run
1.  **Open in Google Colab**: Click the "Open in Colab" badge (available- topmost button ) or upload the `.ipynb` file to your Google Drive and open it with Google Colaboratory.
2.  **Run All Cells**: Navigate to `Runtime > Run all` in the Colab menu. This will execute all cells sequentially.
3.  **Execute Cells Individually**: Alternatively, you can run each cell one by one by clicking the "Play" button next to each code cell or by pressing `Shift + Enter`.
4.  **Interact with Visualizations**: After running the visualization cells, you can interact with the generated Plotly 3D figures (rotate, zoom, pan) and use the play/pause controls for animations.

