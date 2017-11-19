project('nano', 'cpp',
        license : 'MIT',
        meson_version : '>0.42.0',
        default_options : ['cpp_std=c++11'])

nano_headers = [
    'nano_function.hpp',
    'nano_observer.hpp',
    'nano_signal_slot.hpp']

# Dependency
nano = declare_dependency(include_directories : [ '.' ])
install_headers(nano_headers, install_dir : 'nano')

executable('test_nano_wow_a_zero_wing_reference', [ 'tests/simple_test.cpp' ])
