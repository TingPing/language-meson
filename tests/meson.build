project('test', 'c',
  version : '0.1.0',
  default_options : ['warning_level=3'])

# Built-in objects
meson.source_root()
build_machine.system()
host_machine.system()
target_machine.system()

# Variables
foo = 'string'
foo = 12314
foo = [1, 2, 3, 4]
foo = bar
foo += 1231
foo = include_directories('foo', kwarg: 'bar', include_directories: 'foo')

# Numbers (Meson only supports integer numbers)
foo = 1 + 2
foo = 3 * 4
foo = 5 % 3
## Hexadecimal literals
foo = 0x0123456789abcdef == 0X0123456789ABCDEF
foo = 0xFF # Lower-case prefix
foo = 0XFF # Upper-case prefix
## Octal literals
foo = 0o755 # Lower-case prefix
foo = 0O755 # Upper-case prefix
## Binary literals
foo = 0b1111011 # Lower-case prefix
foo = 0B1111011 # Upper-case prefix

# Booleans
foo = true
foo = false

# Strings
foo = ''
foo = ''''''
foo = 'string'
foo = '''string2'''
foo = '\n\n\n'
foo = '''\n\n\n'''
foo = '\\n\\n\\n'
foo = '''\\n\\n\\n'''
## String concatenation
combined = foo1 + '_' + foo2
## String path building
joined = 'C:\\foo\\bar' / 'builddir'
## Strings running over multiple lines
blah = '''
afjoakjflajf  # Test
lflkasjf
test\\\\test
test\\test
test\'test
test\atest
test\btest
test\ftest
test\ntest
test\rtest
test\ttest
test\vtest
test\755test
test\xFFtest
test\uFFFFtest
test\UFFFFFFFFtest
test\N{name}test
test\N{name }test
test\N{ name}test
test\N{n a m e}test
'''
## String formatting
foo = '@0@'.format('test')

# Arrays
foo = ['te\'st', 1, 2, '''test''']

# Dictionaries
dict = {'foo': 42, 'bar': 'baz'}

# Function calls
add_global_arguments(['-foo'])
add_global_link_arguments(['-foo'])

# Method calls
gnome = import('gnome') # As is this
gnome.do_something('test')

# If statements (including logical operations)
if true and false
elif false or true
elif true not false
elif (1 in [1, 2])
elif (3 not in [1, 2])
elif foo == 12
elif (foo != 124) and (foo <= 200)
else
endif

# Foreach statements (including break and continue)
foreach foo : bar
  if foo == 'continue'
    continue
  elif foo == 'break'
    break
  endif
  message(foo)
endforeach

# Comments
some_function() # This is a comment test('foo')
## This is another comment
executable('myexe',
  # This is a comment inside a function call
  'foo.c')

# Ternary operator
foo = true ? 'true' : 'false'
