# semantic-segmentation-benchmarking

# Semantic Segmentation Benchmarking

Inference-only benchmarking of semantic segmentation models for accuracy-latency trade-off analysis.

## Models
- DeepLabV3-ResNet50
- FCN-ResNet50
- DeepLabV3-MobileNetV3-Large
- LRASPP-MobileNetV3-Large

## Dataset
PASCAL VOC 2012 validation set (1,449 images)

## Hardware
NVIDIA Tesla T4 (Google Colab free tier)

## Key Results (512×512)

| Model | mIoU | Latency (ms) | FPS | Params (M) |
|-------|------|-------------|-----|------------|
| DeepLabV3-ResNet50 | 0.7636 | 129.57 | 7.72 | 42.00 |
| FCN-ResNet50 | 0.6987 | 80.20 | 12.43 | 35.32 |
| DeepLabV3-MobileNetV3 | 0.7225 | 15.02 | 63.36 | 11.03 |
| LRASPP-MobileNetV3 | 0.7052 | 6.52 | 146.03 | 3.22 |

## Quick Start
1. Open `code/benchmark_pipeline.ipynb` in Google Colab
2. Runtime → Change runtime type → GPU (T4)
3. Run all cells
4. Results saved to `/content/benchmark_results/`

## Files
- `code/` - Benchmarking notebook
- `results/` - CSV output
- `figures/` - Publication-quality plots

## License
MIT
