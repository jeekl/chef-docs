.. This is an included how-to. 


The |chef server| provides three files that are required by the workstation when connecting to the |chef server|. For the open source |chef server|, log on and download the following files:

* |knife rb|. This configuration file must be created by the user of the open source |chef server|. The ``validation_key`` attribute in the |knife rb| must contain the validation key. The ``validation_client_name`` attribute defaults to ``chef-validator`` (which is the |organization pem| private key created by the open source |chef server| on startup).
* |organization pem|. This private key is created by the open source |chef server| on startup and is located in the |path chef etc| folder on the server after it is created.
* |user pem|. This private key is created by running the ``knife configure --initial`` command.
