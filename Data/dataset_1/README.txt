AIMI dataset_1 (chest X-rays, detection/classification)
Subsampled from the full original; images kept at native 1024x1024 resolution.
train=3000 / val=1500 / test=1500 patients, ~3:1 neg:pos.
train_labels.csv, val_labels.csv: patientId,x,y,width,height,class,PatientAge,PatientSex,ViewPosition,BodyPartExamined,Modality,Target (boxes in 1024px space).
sample_submission.csv: patientId,PredictionString (one row per image, empty predictions).
  PredictionString = 'confidence x y width height' per box, e.g. '0.5 0 0 100 100',
  space-joined for multiple boxes; empty for no predicted pneumonia. Boxes in 1024px space.
