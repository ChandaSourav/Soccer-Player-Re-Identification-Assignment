# Soccer-Player-Re-Identification-Assignment

Cross-Camera Player Mapping<br>
Re-Identification in a Single Feed

# ⚽ Soccer Player Re-Identification — Cross-Camera Mapping (Option 1)

---

## 🛠️ How to Set Up and Run the Code

1. **Upload Required Files** to your environment (e.g., Kaggle or local Jupyter):
   - `broadcast.mp4`
   - `tacticam.mp4`
   - `best.pt` (YOLOv11 model trained for player & ball detection)

2. **Run the Jupyter notebook** or script with the following main steps:
   - Load the YOLO model (`best.pt`)
   - Run detection on both videos using `detect_players(...)`
   - Extract features from player crops using `extract_features(...)`
   - Match players using `match_players(...)`
   - Save the mapping result as a JSON file

3. **Expected Output**:
   - JSON file: `match1.json` containing matched player IDs between both camera views.

---

## 📦 Dependencies / Environment Requirements

This project requires the following Python packages:

```bash
pip install ultralytics
