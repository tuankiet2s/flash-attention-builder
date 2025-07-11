# Flash Attention Builder

Build flash-attention wheels for any CUDA and PyTorch combination from the official [Dao-AILab/flash-attention](https://github.com/Dao-AILab/flash-attention) repository.

## 🎯 Features

- ✅ **One Click Building** - Simple dropdown inputs
- ✅ **CUDA Selection** - Choose from 11.8 to 12.8 versions  
- ✅ **Multi-Platform** - Windows & Linux builds
- ✅ **Auto Release** - Wheels uploaded to GitHub releases
- ✅ **Proper Naming** - Includes CUDA & PyTorch versions

## 🚀 Usage

1. Go to **[Actions](https://github.com/tuankiet2s/flash-attention-builder/actions)** tab
2. Click **"Flash Attention Builder"**
3. Click **"Run workflow"**
4. Select options:
   - **Version**: Flash attention tag (e.g., `v2.6.3`)
   - **CUDA**: Pick from dropdown (11.8.0 to 12.8.1)
5. Click **"Run workflow"**

## 📊 Build Matrix

**Per run, builds for:**
- 🐍 **Python**: 3.10, 3.11, 3.12
- 🔥 **PyTorch**: 2.4.1, 2.5.1, 2.6.0  
- 💻 **OS**: Ubuntu + Windows (Windows has fewer combinations)
- **Total**: ~12-14 wheel variants per CUDA version

## 📦 Download Wheels

Built wheels are available in [Releases](https://github.com/tuankiet2s/flash-attention-builder/releases):

```bash
# Example wheel names:
flash_attn-2.6.3+cu124torch2.5.1-cp310-cp310-linux_x86_64.whl
flash_attn-2.6.3+cu124torch2.6.0-cp311-cp311-win_amd64.whl
```

## 📋 Installation

```bash
# Download the wheel for your setup and install:
pip install flash_attn-2.6.3+cu124torch2.5.1-cp310-cp310-linux_x86_64.whl

# Or use GitHub CLI:
gh release download v2.6.3-builds --repo tuankiet2s/flash-attention-builder
pip install flash_attn-*.whl
```

## ⚡ Quick Test

Test with GitHub CLI:
```bash
gh workflow run "Flash Attention Builder" \
  --repo tuankiet2s/flash-attention-builder \
  -f version=v2.6.3 \
  -f cuda_version=12.4.1
```

## 🔍 Source

- **Built from**: [Dao-AILab/flash-attention](https://github.com/Dao-AILab/flash-attention)
- **Supports**: All official flash-attention releases 