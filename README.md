# GHARP: Real-time Gaussian Head Animation from Large-scale Reconstruction Prior

This software project accompanies the research paper **GHARP: Real-time Gaussian Head Animation from Large-scale Reconstruction Prior** ([arXiv:2610.10945](https://arxiv.org/abs/2610.10945)).

We present a method that animates 3D Gaussian heads in real time from a few input images of a subject and a driving expression signal. We decouple the problem into an identity stage that builds a representation of the subject's geometry and appearance offline, and an animation stage that predicts expression-dependent residuals on top of it at runtime. The animation network operates in a semantically structured latent space of a pretrained reconstruction model, where expression changes remain spatially contained, making residual prediction efficient. To address the body-pose ambiguity inherent to expression-only driving, a body alignment network learns to align the person's body in the target image with the input reference images, removing the ambiguity from the training signal. Our method achieves state-of-the-art quality on the Ava-256 benchmark while running up to 13&times; faster on A100 GPU with 8&times; fewer Gaussians.

## Generated Samples

The repository provides examples of the results for our models trained on the Internal10K and [Ava-256](https://github.com/facebookresearch/ava-256) datasets.

## Citation

```bibtex
@article{benlalah2026gharp,
  title={GHARP: Real-time Gaussian Head Animation from Large-scale Reconstruction Prior},
  author={Benlalah, Ali and Johari, Sepehr and Vitoria, Patricia and Kappeler, Armin and Sevastopolsky, Artem and Jung, Alexander and Fanelli, Gabriele and Mader, Kevin and Breitenstein, Manuel and Pl{\"u}ss, Claudia and R{\"u}egg, Jan and Biland, Simon and Etterlin, Thomas and Kostiaev, Dmitry and Deschler, Mathias and Amberg, Brian and Martin, Sebastian},
  journal={arXiv preprint arXiv:2610.10945},
  year={2026},
  url={https://arxiv.org/abs/2610.10945v1}
}
```

## License

The code is released under the [LICENSE](LICENSE). The images and videos are released under [LICENSE_DATA](LICENSE_DATA). This project was released to accompany a research paper.
