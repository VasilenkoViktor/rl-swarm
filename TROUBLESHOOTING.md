# 🛠️ Troubleshooting

## ⚠️ Issue: Mismatched Protobuf Gencode/Runtime Versions

When running the node, you may encounter the following error:

```
Detected mismatched Protobuf Gencode/Runtime versions...
```

### ✅ Solution:

1. Check your currently installed version:
   ```bash
   pip show protobuf
   ```

2. Uninstall the existing version and install a stable one:
   ```bash
   pip uninstall protobuf
   pip install protobuf==3.20.3
   ```

3. Restart the node:
   ```bash
   ./run_rl_swarm.sh
   ```

This will help avoid compatibility issues when starting the Gensyn node.
