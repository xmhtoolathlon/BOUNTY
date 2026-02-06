# BOUNTY Development Repository

> 🚧 **Development Branch** - This is the main development repository for BOUNTY (Bounded Optimization for Unified Natural-language Training Yields)

## About BOUNTY

BOUNTY is a reinforcement learning framework with reward validation and optimization capabilities. This repository contains the core implementation.

## 🔧 Development Status

This repository is under active development. Many features are currently being implemented or need fixing.

## 🚀 Quick Start

```bash
# Clone the repository
git clone <repository-url>
cd BOUNTY

# Install dependencies
pip install -r requirements.txt
```

## 📁 Repository Structure

```
BOUNTY/
├── bounty/                
│   ├── deepscaler/        # Scaling utilities
│   ├── verl/              # RL training components
│   └── ...
└── README.md              # This file
```

## ⚠️ Development Notes

- This is a **development version** with incomplete implementations
- Many functions contain FIXME markers indicating issues to address

### 🐛 Known FIXME Issues

- [ ] **bounty/deepscaler/utils.py:84** - Implement Vertex AI initialization and authentication
- [ ] **bounty/deepscaler/utils.py:85** - Configure safety settings for content generation
- [ ] **bounty/deepscaler/utils.py:86** - Set up GenerativeModel with proper system instructions
- [ ] **bounty/deepscaler/utils.py:87** - Implement retry logic with exponential backoff
- [ ] **bounty/deepscaler/utils.py:88** - Add comprehensive error handling for API access issues
- [ ] **bounty/deepscaler/utils.py:89** - Handle rate limiting and quota management
- [ ] **bounty/deepscaler/utils.py:90** - Implement response validation and text extraction
- [ ] **bounty/deepscaler/utils.py:91** - Add support for different generation configurations
- [ ] **bounty/verl/verl/protocol.py:114** - Implement batch dimension folding for efficient processing
- [ ] **bounty/verl/verl/protocol.py:115** - Add validation for batch size compatibility
- [ ] **bounty/verl/verl/protocol.py:116** - Handle edge cases where batch_size is not divisible by new_batch_size
- [ ] **bounty/verl/verl/protocol.py:117** - Optimize memory usage during tensor reshaping
- [ ] **bounty/verl/verl/protocol.py:118** - Add support for different tensor types and shapes
- [ ] **bounty/verl/verl/protocol.py:131** - Implement batch dimension unfolding functionality
- [ ] **bounty/verl/verl/protocol.py:132** - Add support for variable batch dimensions
- [ ] **bounty/verl/verl/protocol.py:133** - Optimize tensor view operations for performance
- [ ] **bounty/verl/verl/protocol.py:134** - Handle non-tensor batch data reshaping properly
- [ ] **bounty/verl/verl/protocol.py:135** - Add error handling for invalid batch dimensions
- [ ] **bounty/verl/verl/protocol.py:252** - we can actually lift this restriction if needed
- [ ] **bounty/verl/verl/rewards/reward_validator.py:13** - Add configuration validation
- [ ] **bounty/verl/verl/rewards/reward_validator.py:14** - Initialize default reward bounds
- [ ] **bounty/verl/verl/rewards/reward_validator.py:18** - Implement range checking for rewards
- [ ] **bounty/verl/verl/rewards/reward_validator.py:19** - Add handling for NaN and Inf values
- [ ] **bounty/verl/verl/rewards/reward_validator.py:24** - Implement reward normalization logic
- [ ] **bounty/verl/verl/rewards/reward_validator.py:44** - Handle edge cases where rewards array is empty
- [ ] **bounty/verl/verl/rewards/reward_validator.py:45** - Add support for variable-length episodes
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:77** - add checkpoint manager
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:159** - Implement model loading with proper initialization context
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:160** - Add support for different model types and configurations
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:161** - Implement memory-efficient model loading for large models
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:162** - Add model validation and compatibility checks
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:165** - Complete model loading implementation
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:166** - Add support for custom model architectures
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:167** - Implement proper dtype and attention configuration
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:170** - Implement gradient checkpointing configuration
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:171** - Add memory usage optimization strategies
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:172** - Configure mixed precision training settings
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:173** - Implement FSDP sharding and wrapping policies
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:174** - Add CPU offloading configuration for memory optimization
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:175** - Set up distributed training parameters properly
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:178** - Initialize FSDP wrapped model
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:301** - add a unified tracking
- [ ] **bounty/verl/verl/trainer/main_ppo.py:59** - Extract and validate prompt and response sequences
- [ ] **bounty/verl/verl/trainer/main_ppo.py:60** - Decode sequences to text format
- [ ] **bounty/verl/verl/trainer/main_ppo.py:61** - Apply appropriate reward function based on data source
- [ ] **bounty/verl/verl/trainer/main_ppo.py:62** - Handle edge cases and error conditions
- [ ] **bounty/verl/verl/trainer/main_ppo.py:67** - Implement batch-wise reward computation
- [ ] **bounty/verl/verl/trainer/main_ppo.py:68** - Add proper error handling and validation

## 🤝 Contributing

1. Pick a FIXME item from the list above
2. Implement the fix
3. Test your implementation
4. Update this README when FIXMEs are resolved
