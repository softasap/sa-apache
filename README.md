sa-apache
==========

[![Build Status](https://travis-ci.org/softasap/sa-apache.svg?branch=master)](https://travis-ci.org/softasap/sa-apache)

This role is used in conjunction with other roles, that require apache installed itself.

Example of usage (all parameters are optional)

Simple

  roles:
    - {
        role: "sa-apache"
      }


Advanced:


  roles:
    - {
        role: "sa-apache",
        apache_mode: "worker", # prefork | worker
        apache2_disable_default: true,
        apache_modules:
          - rewrite
          - ssl
      }




