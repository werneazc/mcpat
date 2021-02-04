import os
#generate mcpat as library
# SConscript(['static_lib/Sconscript'])

env = Environment()
includes = ['src/cache', 'src/cacti',
    'src/cacti/decoder', 'src/core', 'src/iocontrollers', 
    'src/logic', 'src/memoryctrl', 'src']
env['LIBS'] = ['libboost_program_options', 'libboost_serialization', 'mcpat']
env['LIBPATH'] = ['usr/local/lib/', './static_lib']
env['CPPPATH'] = includes

env.Program('mcpat', 'driver.cc', 
                     LIBS = ['mcpat'], LIBPATH = ['static_lib'])