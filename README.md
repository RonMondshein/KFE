# K-Filter Ensemble GNN (KFE-GNN)

## Overview  
KFE-GNN extends the **Triple Filter Ensemble (TFE-GNN)** by introducing **band-pass filters** that explicitly capture **mid-frequency signals** in graphs.  
This enables the model to perform well on **homophilic, heterophilic, and mixed-structure datasets**, without losing stability on simpler graphs.  

## Results  
- **Squirrel (mixed)**: **77.23%** vs. 72.27% (TFE-GNN) → **+5% accuracy gain**  
- **Chameleon (mixed)**: **77.89%** vs. 77.16% (TFE-GNN) → small but consistent improvement  
- **Cora, Cornell, Wisconsin**: Comparable performance to TFE-GNN → no loss in strongly homophilic/heterophilic cases  

## Usage  
```bash
pip install -r requirements.txt
python main.py --dataset Squirrel
