.. image:: https://circleci.com/gh/tprrt/curriculum.svg?style=svg&circle-token=8794b4eb585ada86a0521f8c215903faa223de40
    :alt: Circle badge
    :target: https://app.circleci.com/pipelines/github/tprrt/curriculum

====================================
My reStructuredText Curriculum Vitae
====================================

My brief resume in reStructuredText format as well as a template to produce a file in pdf format.

For more details about me, you can visit my `Linkedin profile <https://linkedin.com/in/thomas-perrot-87643637>`_

----

Use commands below to install required Python modules and to convert the resume to pdf format using the template:

::

   # To install required Python modules
   pip install -r requirements.txt

   # To generate the pdf
   rst2pdf --config=./config.ini ./resume.rst -o ./resume.pdf
