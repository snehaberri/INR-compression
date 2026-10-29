INR compression for scientific or medical volumes (CT/MRI, climate grids).
Problem: storage and transfer of huge volumetric data.
What you’d build: a compression pipeline that stores each volume as a small network.
Why it works: a clear metric (PSNR vs. bits per voxel) and strong baselines to beat (JPEG2000, zfp, SZ).
Risk: it’s crowded, so you need a specific angle, such as shared initialization across a dataset.
Searching and classifying directly in weight space.
Problem: archives of INR-encoded data can’t be searched without decoding every file.
What you’d build: symmetry-aware (alignment-based) embeddings of network weights for retrieval or classification.
Why it works: it extends your research most directly, and it’s less crowded than the others.
Risk: the “big real-world problem” story is weaker, so pair it with option 2 as the storage use case.