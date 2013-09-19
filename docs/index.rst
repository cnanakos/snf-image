.. snf-image documentation master file, created by
   sphinx-quickstart on Fri Sep 13 16:50:13 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to snf-image's documentation!
=====================================

.. image:: /images/logo.png

snf-image is a `Ganeti <http://code.google.com/p/ganeti/>`_ OS definition,
primary used by `Synnefo <http://www.synnefo.org/>`_. It is rewritten from
scratch and allows Ganeti to launch instances from predefined or untrusted
custom Images. The whole process of deploying an Image onto the block device,
as provided by Ganeti, is done in complete isolation from the physical host,
enhancing robustness and security.

snf-image supports `KVM <http://www.linux-kvm.org/page/Main_Page>`_ and
`Xen <http://www.xenproject.org/>`_ based ganeti clusters.

There are also additional hooks that can be enabled at image deployment. They
allow for:

 * changing the password of root or arbitrary users
 * injecting files at arbitrary locations inside the filesystem, e.g., SSH keys
 * setting a custom hostname
 * re-creating SSH host keys to ensure the image uses unique keys

snf-image has been used successfully to deploy many major Linux distributions
(Debian, Ubuntu/Kubuntu, CentOS, Fedora, OpenSUSE), Windows 2008 R2 & Windows
Server 2012, as well as FreeBSD 9.1

The snf-image Ganeti OS Definition is released under
`GPLv2 <http://www.gnu.org/licenses/gpl-2.0.html>`_.



Contents:
^^^^^^^^^

.. toctree::
   :maxdepth: 2

   architecture
   installation
   usage
   advanced

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
