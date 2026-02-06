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

- [ ] **bounty/deepscaler/utils.py:45** - Implement OpenAI API client initialization
- [ ] **bounty/deepscaler/utils.py:46** - Add proper authentication handling
- [ ] **bounty/deepscaler/utils.py:47** - Implement exponential backoff retry logic for rate limits
- [ ] **bounty/deepscaler/utils.py:48** - Add comprehensive error handling for different API errors
- [ ] **bounty/deepscaler/utils.py:49** - Implement response parsing and validation
- [ ] **bounty/deepscaler/utils.py:50** - Add logging for API calls and errors
- [ ] **bounty/deepscaler/utils.py:51** - Support batch processing for multiple prompts
- [ ] **bounty/deepscaler/utils.py:52** - Add timeout configuration for API calls
- [ ] **bounty/deepscaler/utils.py:88** - Implement Vertex AI initialization and authentication
- [ ] **bounty/verl/verl/protocol.py:114** - Implement batch dimension folding for efficient processing
- [ ] **bounty/verl/verl/protocol.py:115** - Add validation for batch size compatibility
- [ ] **bounty/verl/verl/trainer/fsdp_sft_trainer.py:77** - add checkpoint manager
- [ ] **bounty/verl/verl/trainer/main_ppo.py:50** - Implement reward computation for different data sources
- [ ] **bounty/verl/verl/trainer/main_ppo.py:53** - Add support for parallel processing of reward computation
- [ ] **bounty/verl/verl/trainer/main_ppo.py:54** - Implement proper sequence decoding and validation

## 🤝 Contributing

1. Pick a FIXME item from the list above
2. Implement the fix
3. Test your implementation
4. Update this README when FIXMEs are resolved
