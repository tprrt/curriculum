.. image:: https://circleci.com/gh/tprrt/curriculum.svg?style=svg
    :alt: Circle badge
    :target: https://app.circleci.com/pipelines/github/tprrt/curriculum

====================================
My reStructuredText Curriculum Vitae
====================================

My brief resume in reStructuredText format as well as a template to produce a file in pdf format.

For more details about me, you can visit my `Linkedin`_ profile.

----

Use commands below to install required Python modules and to convert the resume to pdf format using the template:

::

    # To create a Python3 virtual environment
    python3 -m venv venv
    . venv/bin/activate

    # To install required Python modules
    pip install -r requirements.txt

    # To generate in the PDF format
    rst2pdf --config=./config.ini ./resume.rst -o resume.pdf

    # To quit the Python3 virtual environment
    deactivate


----

Use the following command to validate the `circleci`_ pipeline:

::

    podman run --rm --security-opt seccomp=unconfined --security-opt label=disable -v $(pwd):/data circleci/circleci-cli:alpine config validate /data/.circleci/config.yml --token $TOKEN


.. _circleci: https://circleci.com
.. _Linkedin: https://www.linkedin.com/in/tprrt
