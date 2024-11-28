
npm run build
npm run start
cd ecom-proj-master
git ls-files --stage | grep 160000
git submodule status
conda deactivate
django-admin --version
(base) PS D:\telusko> conda deactivate
PS D:\telusko> django-admin --version
5.0.3
PS D:\telusko> python -m venv test
PS D:\telusko> test\Scripts\activate
(test) PS D:\telusko> cd D:\telusko\projects\telusko
(test) PS D:\telusko\projects\telusko> python manage.py runserver
    from django.core.management import execute_from_command_line
ModuleNotFoundError: No module named 'django'

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "D:\telusko\projects\telusko\manage.py", line 22, in <module>
    main()
  File "D:\telusko\projects\telusko\manage.py", line 13, in main
    raise ImportError(
ImportError: Couldn't import Django. Arpip install djangostalled and available on your PYTHONPATH environment variable? Did you forget to activate a virtual environment?
>> st) PS D:\telusko\projects\telusko>
Collecting django
  Obtaining dependency information for django from https://files.pythonhosted.org/packages/a3/b8/f205f2b8c44c6cdc555c4f56bbe85ceef7f67c0cf1caa8abe078bb7e32bd/Django-5.1.2-py3-none-any.whl.metadata
  Downloading Django-5.1.2-py3-none-any.whl.metadata (4.2 kB)
Collecting asgiref<4,>=3.8.1 (from django)
  Obtaining dependency information for asgiref<4,>=3.8.1 from https://files.pythonhosted.org/packages/39/e3/893e8757be2612e6c266d9bb58ad2e3651524b5b40cf56761e985a28b13e/asgiref-3.8.1-py3-none-any.whl.metadata
  Using cached asgiref-3.8.1-py3-none-any.whl.metadata (9.3 kB)
Collecting sqlparse>=0.3.1 (from django)
  Obtaining dependency information for sqlparse>=0.3.1 from https://files.pythonhosted.org/packages/5d/a5/b2860373aa8de1e626b2bdfdd6df4355f0565b47e51f7d0c54fe70faf8fe/sqlparse-0.5.1-py3-none-any.whl.metadata
  Downloading sqlparse-0.5.1-py3-none-any.whl.metadata (3.9 kB)
Collecting tzdata (from django)
  Obtaining dependency information for tzdata from https://files.pythonhosted.org/packages/a6/ab/7e5f53c3b9d14972843a647d8d7a853969a58aecc7559cb3267302c94774/tzdata-2024.2-py2.py3-none-any.whl.metadata
  Downloading tzdata-2024.2-py2.py3-none-any.whl.metadata (1.4 kB)
Downloading Django-5.1.2-py3-none-any.whl (8.3 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.3/8.3 MB 3.6 MB/s eta 0:00:00
Using cached asgiref-3.8.1-py3-none-any.whl (23 kB)
Downloading sqlparse-0.5.1-py3-none-any.whl (44 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 44.2/44.2 kB 2.1 MB/s eta 0:00:00
Downloading tzdata-2024.2-py2.py3-none-any.whl (346 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 346.6/346.6 kB 10.5 MB/s eta 0:00:00
Installing collected packages: tzdata, sqlparse, asgiref, django       
Successfully installed asgiref-3.8.1 django-5.1.2 sqlparse-0.5.1 tzdata-2024.2

[notice] A new release of pip is available: 23.2.1 -> 24.2
[notice] To update, run: python.exe -m pip install --upgrade pip       
(test) PS D:\telusko\projects\telusko> pip install django
>>                                     pip install django
                                                         
(test) PS D:\telusko\projects\telusko> python manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
 
