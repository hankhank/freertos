import os
import sys
import time

Import('env')

env = env.Clone()
env['CPPPATH'].append('portable/GCC/ARM_CM3/')

freertosfile = [
    Glob('*.c'),
    'portable/GCC/ARM_CM3/port.c',
    'portable/MemMang/heap_3.c'
]

# Unit tests
freertos = env.StaticLibrary('freertos', freertosfile)

Return('freertos')
