# AICS-202 Adversarial Machine Learning - Integrated Assessment

Student: Firdaws Alnuur Mohammed | ID: 2026/AICDF/16701    

## Environment (verified 12 Nov 2026)
- OS: Linux x86_64 (glibc 2.39); 1 CPU core, ~3.9 GB RAM, no GPU
- Python: 3.12.3 (virtual environment `.venv`)
- Libraries (from requirements.txt, resolved versions):
  numpy 2.5.4, scikit-learn 1.9.1, matplotlib 3.11.2, notebook 7.6.5,
  nbconvert 7.17.2, nbclient 0.11.0, ipykernel 7.4.0
- Full pinned list: `pip_freeze.txt`
- Dataset: `sklearn.datasets.load_digits()`; verified shape (1797, 64), 10 classes,
  raw pixel range 0-16 (scaled to 0-1 in the notebooks). No downloads required.

## Seeds
- 42: train/test split (stratified, test_size=0.25) and LogisticRegression/PGD start
- 2026: label-poisoning RNG (Lab 03)

## Run commands
    python -m venv .venv && . .venv/bin/activate
    python -m pip install -r requirements.txt
    jupyter nbconvert --to notebook --execute --inplace Lab01_...ipynb   # repeat for 02-04
(Each notebook is also runnable via Restart and Run All in Jupyter.)

## Layout
- Labs/*.ipynb (executed, outputs saved), results/ (exported charts), evidence/ (E01-E05)
- AICS202_Final_Report.pdf, threat model, integrity register, decision memo

## AI assistance
See the AI-assistance declaration (to be completed at the end, honestly, from the
log in evidence/ai_assistance_log.md).

