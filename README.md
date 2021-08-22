<p><a href="https://www.buymeacoffee.com/banterless" target="_blank"><img style="height: 41px !important; width: 174px !important; box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important; -webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" /></a></p>
<p>This repository contains the official TensorFlow 2.x implementation, in Jupyter Notebook, of the following paper:</p>
<blockquote>
<p><strong>An Image-based Generator Architecture for Synthetic Image Refinement</strong><br />Alex Nasser<br /><a href="https://arxiv.org/abs/2108.04957" rel="nofollow">https://arxiv.org/abs/2108.04957</a></p>
<p><strong>Abstract:</strong> <em>Proposed are alternative generator architectures for Boundary Equilibrium Generative Adversarial Networks (BEGAN), motivated by Learning from Simulated and Unsupervised Images through Adversarial Training (SimGAN). It disentangles the need for a noise-based latent space. The generator will operate mainly as a refiner network to gain a photo-realistic presentation of the given synthetic images. It also attempts to resolve the latent space's poorly understood properties by eliminating the need for noise injection and replacing it with an image-based concept. The new flexible and simple generator architecture will also give the power to control the trade-off between restrictive refinement and expressiveness ability. Contrary to other available methods, this architecture will not require a paired or unpaired dataset of real and synthetic images for the training phase. Only a relatively small set of real images would suffice.</em></p>
</blockquote>
<p><img style="max-width: 65%;" src="https://user-images.githubusercontent.com/44167267/129492992-7f46b08b-4a01-438d-88b6-a3f2ecac0776.png" alt=""  /></p>
<h2><a id="user-content-usage" class="anchor" aria-hidden="true" href="#usage"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Usage</h2>
<p>Use your own dataset</p>
<pre><code>dataset
└── real images (you would need at least 20k real-life portrait face pictures in this folder )
    ├── xxx.jpg (the name doesn't matter)
    ├── yyy.jpg
    └── ...
└── synthetic images (use this folder to store 3d or even 2d generated synthetic images for model evaluation)
    ├── xxx.jpg (the name doesn't matter)
    ├── yyy.jpg
    └── ...
</code></pre>
<h3><a id="user-content-train" class="anchor" aria-hidden="true" href="#train"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Train</h3>
<p>Run model.ipynb in Juypyter Notebook to train and evaluate the mode</p>
