# Q-VGM: Q-Value-Gradient Matching for Off-Policy Reinforcement Learning of Flow-Matching VLA

Official repository for **Q-VGM**, an off-policy RL method that fine-tunes flow-matching
vision-language-action (VLA) policies with a learned Q-function — no action likelihoods,
no backpropagation through the denoising chain, and the critic is discarded at inference.

📄 Paper: [arXiv:2606.08015](https://arxiv.org/abs/2606.08015)

## Highlights

- **BPTT-free Q-learning for flow policies**: critic-improved actions are converted into
  velocity-space supervision of the action expert.
- **Offline-to-online**: IQL critic in the offline phase, standard TD online, on the same
  $\pi_{0.5}$ backbone.
- **Results**: LIBERO few-shot SFT 86.9% → 93.0% (offline, 150 episodes/task) → 100%
  (online, ~6× fewer rollout episodes than PPO); three real bimanual tasks 66.7% → 98.3%.

## Code

Code will be released soon.

## Citation

```bibtex
@article{wang2026qvgm,
  title={Q-VGM: Q-Value-Gradient Matching for Off-Policy Reinforcement Learning of Flow-Matching VLA},
  author={Wang, Ziqian and Qu, Chendi and Sun, Jiayu and Liu, Yitian and Mao, Xingjian and Wang, Minqian and Mu, Yao},
  journal={arXiv preprint arXiv:2606.08015},
  year={2026}
}
```
