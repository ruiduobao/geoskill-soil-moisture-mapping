---
name: geoskill-soil-moisture-mapping
description: '用热惯量法与 SAR Dubois 模型估算表层土壤湿度并划分干旱等级。Estimates surface soil moisture via thermal inertia and the SAR Dubois model, with drought grading.'
---

# 土壤湿度制图 | Soil Moisture Mapping

(Fill in 2-3 paragraphs of Chinese introduction here: features, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'scipy'
```

## Usage / 使用方法

### Basic Usage

```bash
python geoskill-soil-moisture-mapping.py --bbox 116.0 39.0 117.0 40.0 [other parameters]
```

### Example 1 (Synthetic Data, Offline)

```bash
python geoskill-soil-moisture-mapping.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real-world usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Main output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is done locally; no user data is uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
