# Copyright 2015 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

python_library(
  name='plugin',
  sources=['register.py'],
  dependencies=[
    'contrib/scrooge/src/python/pants/contrib/scrooge/tasks',
    'src/python/pants/goal:task_registrar',

    # TODO(John Sirois): Remove this once setup-py learns to index providers that are out of scope.
    # see: https://github.com/pantsbuild/pants/issues/1329
    'src/python/pants:pants-packaged',
  ],
  provides=contrib_setup_py(
    name='pantsbuild.pants.contrib.scrooge',
    description='Scrooge thrift generator pants plugins.',
    additional_classifiers=[
      'Topic :: Software Development :: Code Generators'
    ]
  )
)
