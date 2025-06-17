# Image Dataset - 2025-06-17 Acquisition

This dataset contains TIFF images captured on 2025-06-17 with two different exposure settings.

## Dataset Structure

```
dataset/
├── 2025-06-17 acquisition/
│   ├── exposure10000/     # Images with 20k exposure setting
│   └── exposure20000/     # Images with 40k exposure setting
```

## Statistics

- **Total Size**: ~13.14 GB
- **Total Files**: 380 TIFF images
- **Exposure Settings**: 10000 and 20000
- **File Format**: TIFF

## Usage

These images are stored using Git LFS (Large File Storage) due to their size.

### 🚨 Important: Cloning Instructions

**You MUST have Git LFS installed to properly download the images:**

```bash
# 1. Install Git LFS (one-time setup)
git lfs install

# 2. Clone the repository (this downloads image pointers, not full files)
git clone <repository-url>
cd <repository-name>

# 3. Download the actual image files (13.14 GB download)
git lfs pull
```

### Alternative: Clone with LFS files immediately

```bash
# Install Git LFS first
git lfs install

# Clone and download all LFS files in one command
git clone <repository-url>
# LFS files are automatically downloaded during clone if LFS is installed
```

### Verification

Check that you have the actual images (not just pointers):

```bash
# Image files should be ~35MB each, not just a few bytes
ls -lh "2025-06-17 acquisition/exposure10000/grabbed_image_101.tiff"
```

### ⚠️ Download Warning

- **Full dataset**: 13.14 GB
- **Time**: Depends on your internet connection
- **Storage**: Ensure you have enough disk space

## File Naming Convention

Images follow the pattern: `grabbed_image_[number].tiff`

## Notes

⚠️ **Important**: This repository uses Git LFS which has bandwidth limits on GitHub. Consider the costs and limitations before downloading the full dataset multiple times.
