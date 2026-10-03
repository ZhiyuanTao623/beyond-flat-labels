# Beyond Flat Labels: Level-Restricted Contrastive Learning for Hierarchical Fine-Grained Vision Classification

Project page for the paper, accepted to the CVPR 2026 FGVC Workshop.

- Paper: [arXiv:2606.21838](https://arxiv.org/abs/2606.21838) ([PDF](https://arxiv.org/pdf/2606.21838))
- Models: [BioCLIP-HC-Euclidean](https://huggingface.co/imageomics/bioclip-hc-euclidean), [BioCLIP-HC-Hyperbolic](https://huggingface.co/imageomics/bioclip-hc-hyperbolic)
- Project page: https://zhiyuantao623.github.io/beyond-flat-labels/

## Summary

CLIP-style vision-language models often predict a species whose genus, family or order contradicts what the same model predicts at those higher levels. The cause is false negatives that appear when labels from different taxonomic levels share one contrastive objective. Level-restricted contrastive learning contrasts each label only against labels of the same taxonomic level and weights all levels equally.

Fine-tuned from BioCLIP on TreeOfLife-10M, the models reach 78.96% average top-1 accuracy over seven taxonomic levels on iNat21 (BioCLIP: 48.49%) and a normalized LCA of 0.71 under top-down constrained inference (RCME: 0.43, BioCLIP: 0.32), in both Euclidean and hyperbolic embedding spaces.

## Citation

```bibtex
@article{tao2026beyondflatlabels,
  title   = {Beyond Flat Labels: Level-Restricted Contrastive Learning for Hierarchical Fine-Grained Vision Classification},
  author  = {Tao, Zhiyuan and Sastry, Srikumar and Thompson, Matthew J and Campolongo, Elizabeth G and Zhang, Net and Zhang, Ziheng and Lapp, Hilmar and Su, Yu and Berger-Wolf, Tanya and Jacobs, Nathan and Chao, Wei-Lun and Gu, Jianyang},
  journal = {arXiv preprint arXiv:2606.21838},
  year    = {2026},
  note    = {Accepted to the CVPR 2026 FGVC Workshop}
}
```

## Files

- `index.html`: the page (self-contained; no build step)
- `llms.txt`, `llms-full.txt`: plain-text summaries for language models and agents
- `robots.txt`, `sitemap.xml`: crawler hints
- `assets/`: figures from the paper
