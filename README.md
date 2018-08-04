## Using pyMatlab as Bridge betweeen Matlab and Python
These instruction would give explanation about installation of pymatlab via pip and using 

### Prerequisites
Install pymatlab
```
pip install pymatlab
```

## Using pyMatlab

### Importing
```
import pymatlab
```

### Intializing engine
```
matlab_sess = pymatlab.session_factory(options = '-nodesktop -nosplash')
```

### Run Matlab commands as from python in this engine
Change path
```
matlab_sess.run('path/to/folders/')
```

### Push values to matlab from python
```
matlab_sess.putvalue('V1',p_mat_image)
```

### Running functions
```
matlab_sess.run('c_p=shape_context_warp_func(V1,V2)')
```

### Fetching values from Matlab
```
tps_control_points = matlab_sess.getvalue('c_p')
```
