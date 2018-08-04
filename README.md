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
matlab_sess.putvalue('*variable_as_in_matlab*',python_variables)
```

### Running functions
```
matlab_sess.run('name_of_the_.m_file(matlab_variable1,matlab_variable2)')
```

### Fetching values from Matlab
```
tps_control_points = matlab_sess.getvalue('c_p')
```
