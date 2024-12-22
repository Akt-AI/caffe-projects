```markdown
# ReadMe

## Build Caffe for CPU on Ubuntu 18.04

Follow these steps to build Caffe on Ubuntu 18.04:

### Step 1: Create a Virtual Environment
Run the following command to create a virtual environment:
```bash
virtualenv -p python3.6 env3.6
```

### Step 2: Make the Build Script Executable
```bash
chmod +x build_caffe.sh
```

### Step 3: Clone the Caffe Repository
```bash
git clone https://github.com/BVLC/caffe.git
```

### Step 4: Copy the Build Script
Copy `build_caffe.sh` into the `caffe-master` directory:
```bash
cp build_caffe.sh caffe-master/
```

### Step 5: Run the Build Script
Navigate to the `caffe-master` directory and execute the build script:
```bash
cd caffe-master
./build_caffe.sh
```

The above commands will automatically install all dependencies and build Caffe.

---

### Step 6: Run the Caffe Python API
Activate the virtual environment and set the Python path:
```bash
source env3.6/bin/activate
export PYTHONPATH=./python
```

### Step 7: Test the Python API
Run Python and test the Caffe API:
```bash
python
>>> import caffe
>>> print(dir(caffe))
```

You should see a list of available Caffe modules.

---

Enjoy using Caffe on Ubuntu 18.04!
```
