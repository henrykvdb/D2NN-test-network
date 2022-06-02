# D2NN-test-network

The blocks are set up as ResNet basic blocks, with batch-
norms and ReLU layers in between.
• Conv 0: (3x3 conv, 3 → 64)
• Block 1: (3x3 conv, 64 → 64), (3x3 conv, 64 → 64)
• Block 2: (3x3 conv, 64 → 64), (3x3 conv, 64 → 64)
• Block 3: (3x3 conv, 64 → 128, stride 2), (3x3 conv, 128 → 128), (1x1 conv, 64 → 128, stride 2)
• Block 4: (3x3 conv, 128 → 128), (3x3 conv, 128 → 128)
• Block 5: (3x3 conv, 128 → 256, stride 2), (3x3 conv, 256 → 256), (1x1 conv, 128 → 256, stride 2)
• Block 6: (3x3 conv, 256 → 256), (3x3 conv, 256 → 256)
• Block 7: (3x3 conv, 256 → 512, stride 2), (3x3 conv, 512 → 512), (1x1 conv, 256 → 512, stride 2)
• Block 8: (3x3 conv, 512 → 512), (3x3 conv, 512 → 512)
• Classifier: 4x4 average pool, 512 → 100 fully connected
• Block 4*: (3x3 conv, 128 → 128, stride 2), (3x3 conv, 128 → 128), (1x1 conv, 128 → 128, stride 2)
• Block 6*: (3x3 conv, 256 → 256, stride 2), (3x3 conv, 256 → 256), (1x1 conv, 256 → 256, stride 2)
• Classifier*: 4x4 average pool, 256 → 100 fully connected
