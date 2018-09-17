-------------------------------------
/var/log/httpd/error_log
-------------------------------------
[Mon Sep 17 23:29:33.567252 2018] [suexec:notice] [pid 2514] AH01232: suEXEC mechanism enabled (wrapper: /usr/sbin/suexec)
[Mon Sep 17 23:29:33.720956 2018] [http2:warn] [pid 2514] AH10034: The mpm module (prefork.c) is not supported by mod_http2. The mpm determines how things are processed in your server. HTTP/2 has more demands in this regard and the currently selected mpm will just not do. This is an advisory warning. Your server will continue to work, but the HTTP/2 protocol will be inactive.
[Mon Sep 17 23:29:33.720990 2018] [http2:warn] [pid 2514] AH02951: mod_ssl does not seem to be enabled
[Mon Sep 17 23:29:33.722167 2018] [lbmethod_heartbeat:notice] [pid 2514] AH02282: No slotmem from mod_heartmonitor
[Mon Sep 17 23:29:33.722300 2018] [:warn] [pid 2514] mod_wsgi: Compiled for Python/3.6.2.
[Mon Sep 17 23:29:33.722325 2018] [:warn] [pid 2514] mod_wsgi: Runtime using Python/3.6.5.
[Mon Sep 17 23:29:33.739744 2018] [mpm_prefork:notice] [pid 2514] AH00163: Apache/2.4.33 (Amazon) mod_wsgi/3.5 Python/3.6.5 configured -- resuming normal operations
[Mon Sep 17 23:29:33.739800 2018] [core:notice] [pid 2514] AH00094: Command line: '/usr/sbin/httpd -D FOREGROUND'
[Mon Sep 17 23:30:18.157840 2018] [mpm_prefork:notice] [pid 2514] AH00169: caught SIGTERM, shutting down
[Mon Sep 17 23:30:19.290335 2018] [suexec:notice] [pid 2772] AH01232: suEXEC mechanism enabled (wrapper: /usr/sbin/suexec)
[Mon Sep 17 23:30:19.322296 2018] [so:warn] [pid 2772] AH01574: module wsgi_module is already loaded, skipping
[Mon Sep 17 23:30:19.326017 2018] [http2:warn] [pid 2772] AH10034: The mpm module (prefork.c) is not supported by mod_http2. The mpm determines how things are processed in your server. HTTP/2 has more demands in this regard and the currently selected mpm will just not do. This is an advisory warning. Your server will continue to work, but the HTTP/2 protocol will be inactive.
[Mon Sep 17 23:30:19.326036 2018] [http2:warn] [pid 2772] AH02951: mod_ssl does not seem to be enabled
[Mon Sep 17 23:30:19.327042 2018] [lbmethod_heartbeat:notice] [pid 2772] AH02282: No slotmem from mod_heartmonitor
[Mon Sep 17 23:30:19.327185 2018] [:warn] [pid 2772] mod_wsgi: Compiled for Python/3.6.2.
[Mon Sep 17 23:30:19.327198 2018] [:warn] [pid 2772] mod_wsgi: Runtime using Python/3.6.5.
[Mon Sep 17 23:30:19.337632 2018] [mpm_prefork:notice] [pid 2772] AH00163: Apache/2.4.33 (Amazon) mod_wsgi/3.5 Python/3.6.5 configured -- resuming normal operations
[Mon Sep 17 23:30:19.337678 2018] [core:notice] [pid 2772] AH00094: Command line: '/usr/sbin/httpd -D FOREGROUND'



-------------------------------------
/opt/python/log/supervisord.log
-------------------------------------
2018-09-17 23:29:30,947 CRIT Supervisor running as root (no user in config file)
2018-09-17 23:29:30,983 INFO RPC interface 'supervisor' initialized
2018-09-17 23:29:30,983 CRIT Server 'unix_http_server' running without any HTTP authentication checking
2018-09-17 23:29:30,984 INFO supervisord started with pid 2464
2018-09-17 23:29:31,986 INFO spawned: 'httpd' with pid 2514
2018-09-17 23:29:32,994 INFO success: httpd entered RUNNING state, process has stayed up for > than 1 seconds (startsecs)
2018-09-17 23:30:18,173 INFO stopped: httpd (exit status 0)
2018-09-17 23:30:19,182 INFO spawned: 'httpd' with pid 2772
2018-09-17 23:30:20,289 INFO success: httpd entered RUNNING state, process has stayed up for > than 1 seconds (startsecs)



-------------------------------------
/var/log/httpd/access_log
-------------------------------------
127.0.0.1 (-) - - [17/Sep/2018:23:30:22 +0000] "GET / HTTP/1.1" 200 3462 "-" "Python-urllib/2.7"
54.39.10.49 (-) - - [17/Sep/2018:23:36:51 +0000] "GET / HTTP/1.0" 200 3462 "-" "masscan/1.0 (https://github.com/robertdavidgraham/masscan)"



-------------------------------------
/var/log/eb-activity.log
-------------------------------------
[2018-09-17T23:29:30.255Z] INFO  [2273]  - [Initialization] : Completed activity. Result:
  Initialization - Command CMD-PreInit succeeded
[2018-09-17T23:30:09.097Z] INFO  [2630]  - [Application deployment Sample Application@1] : Starting activity...
[2018-09-17T23:30:09.098Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore] : Starting activity...
[2018-09-17T23:30:09.098Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore/ConfigCWLAgent] : Starting activity...
[2018-09-17T23:30:09.098Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore/ConfigCWLAgent/10-config.sh] : Starting activity...
[2018-09-17T23:30:09.348Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore/ConfigCWLAgent/10-config.sh] : Completed activity. Result:
  Log streaming option setting is not specified, ignore cloudwatch logs setup.
  
  Disabled log streaming.
[2018-09-17T23:30:09.348Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore/ConfigCWLAgent] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/addons/logstreaming/hooks/config.
[2018-09-17T23:30:09.349Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsBefore] : Completed activity.
[2018-09-17T23:30:10.073Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0] : Starting activity...
[2018-09-17T23:30:10.073Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdLogRotation] : Starting activity...
[2018-09-17T23:30:10.086Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdLogRotation] : Completed activity. Result:
  ["/etc/cron.hourly/cron.logrotate.elasticbeanstalk.healthd.conf"]
[2018-09-17T23:30:10.086Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdHTTPDLogging] : Starting activity...
[2018-09-17T23:30:10.087Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdHTTPDLogging] : Completed activity.
[2018-09-17T23:30:10.087Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdNginxLogging] : Starting activity...
[2018-09-17T23:30:10.087Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/HealthdNginxLogging] : Completed activity.
[2018-09-17T23:30:10.087Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild] : Starting activity...
[2018-09-17T23:30:10.832Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild/Infra-EmbeddedPreBuild] : Starting activity...
[2018-09-17T23:30:10.838Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild/Infra-EmbeddedPreBuild/prebuild_0_AWS_Beanstalk_Web_App_Python_1_Sample] : Starting activity...
[2018-09-17T23:30:10.839Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild/Infra-EmbeddedPreBuild/prebuild_0_AWS_Beanstalk_Web_App_Python_1_Sample] : Completed activity.
[2018-09-17T23:30:10.839Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild/Infra-EmbeddedPreBuild] : Completed activity.
[2018-09-17T23:30:10.871Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPreBuild] : Completed activity.
[2018-09-17T23:30:10.871Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook] : Starting activity...
[2018-09-17T23:30:10.871Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/01_configure_xray.sh] : Starting activity...
[2018-09-17T23:30:11.095Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/01_configure_xray.sh] : Completed activity.
[2018-09-17T23:30:11.095Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/01new.py] : Starting activity...
[2018-09-17T23:30:11.775Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/01new.py] : Completed activity.
[2018-09-17T23:30:11.775Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/02unzip.py] : Starting activity...
[2018-09-17T23:30:12.469Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/02unzip.py] : Completed activity. Result:
  Archive:  /opt/elasticbeanstalk/deploy/appsource/source_bundle
    inflating: /opt/python/ondeck/app/application.py  
    inflating: /opt/python/ondeck/app/cron.yaml  
[2018-09-17T23:30:12.469Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/03deploy.py] : Starting activity...
[2018-09-17T23:30:12.957Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/03deploy.py] : Completed activity.
[2018-09-17T23:30:12.957Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/04configen.py] : Starting activity...
[2018-09-17T23:30:15.637Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook/04configen.py] : Completed activity.
[2018-09-17T23:30:15.637Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/AppDeployPreHook] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/hooks/appdeploy/pre.
[2018-09-17T23:30:15.638Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPostBuild] : Starting activity...
[2018-09-17T23:30:16.395Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPostBuild/Infra-EmbeddedPostBuild] : Starting activity...
[2018-09-17T23:30:16.395Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPostBuild/Infra-EmbeddedPostBuild] : Completed activity.
[2018-09-17T23:30:16.424Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/EbExtensionPostBuild] : Completed activity.
[2018-09-17T23:30:16.424Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/InfraCleanEbExtension] : Starting activity...
[2018-09-17T23:30:16.425Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0/InfraCleanEbExtension] : Completed activity. Result:
  Cleaned ebextensions subdirectories from /opt/python/ondeck/app.
[2018-09-17T23:30:16.426Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage0] : Completed activity. Result:
  Application deployment - Command CMD-Startup stage 0 completed
[2018-09-17T23:30:16.426Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1] : Starting activity...
[2018-09-17T23:30:16.426Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook] : Starting activity...
[2018-09-17T23:30:16.427Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/01flip.py] : Starting activity...
[2018-09-17T23:30:22.599Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/01flip.py] : Completed activity. Result:
  httpd: stopped
  httpd: started
  httpd                            RUNNING   pid 2772, uptime 0:00:03
[2018-09-17T23:30:22.599Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/01stop_xray.sh] : Starting activity...
[2018-09-17T23:30:24.850Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/01stop_xray.sh] : Completed activity. Result:
  Executing: if ( initctl status xray | grep start ); then initctl stop xray; fi
  xray start/running, process 1712
  xray stop/waiting
[2018-09-17T23:30:24.851Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/02create_pids_for_monitoring.sh] : Starting activity...
[2018-09-17T23:30:25.083Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/02create_pids_for_monitoring.sh] : Completed activity. Result:
  + chmod 0755 /var/run/httpd
  + /opt/elasticbeanstalk/bin/healthd-track-pidfile --proxy httpd
  + /opt/elasticbeanstalk/bin/healthd-track-pidfile --name application --location /opt/python/run/supervisord.pid
[2018-09-17T23:30:25.083Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/02start_xray.sh] : Starting activity...
[2018-09-17T23:30:25.303Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook/02start_xray.sh] : Completed activity.
[2018-09-17T23:30:25.304Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployEnactHook] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/hooks/appdeploy/enact.
[2018-09-17T23:30:25.304Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployPostHook] : Starting activity...
[2018-09-17T23:30:25.304Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/AppDeployPostHook] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/hooks/appdeploy/post.
[2018-09-17T23:30:25.304Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/PostInitHook] : Starting activity...
[2018-09-17T23:30:25.305Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/PostInitHook/01processmgrstart.sh] : Starting activity...
[2018-09-17T23:30:25.315Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/PostInitHook/01processmgrstart.sh] : Completed activity. Result:
  + pgrep supervisord
  2464
[2018-09-17T23:30:25.315Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1/PostInitHook] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/hooks/postinit.
[2018-09-17T23:30:25.315Z] INFO  [2630]  - [Application deployment Sample Application@1/StartupStage1] : Completed activity. Result:
  Application deployment - Command CMD-Startup stage 1 completed
[2018-09-17T23:30:25.316Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter] : Starting activity...
[2018-09-17T23:30:25.316Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter/ConfigLogRotation] : Starting activity...
[2018-09-17T23:30:25.316Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter/ConfigLogRotation/10-config.sh] : Starting activity...
[2018-09-17T23:30:25.483Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter/ConfigLogRotation/10-config.sh] : Completed activity. Result:
  Disabled forced hourly log rotation.
[2018-09-17T23:30:25.484Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter/ConfigLogRotation] : Completed activity. Result:
  Successfully execute hooks in directory /opt/elasticbeanstalk/addons/logpublish/hooks/config.
[2018-09-17T23:30:25.484Z] INFO  [2630]  - [Application deployment Sample Application@1/AddonsAfter] : Completed activity.
[2018-09-17T23:30:25.484Z] INFO  [2630]  - [Application deployment Sample Application@1] : Completed activity. Result:
  Application deployment - Command CMD-Startup succeeded
[2018-09-17T23:50:07.615Z] INFO  [3460]  - [CMD-TailLogs] : Starting activity...
[2018-09-17T23:50:07.615Z] INFO  [3460]  - [CMD-TailLogs/AddonsBefore] : Starting activity...
[2018-09-17T23:50:07.615Z] INFO  [3460]  - [CMD-TailLogs/AddonsBefore] : Completed activity.
[2018-09-17T23:50:07.615Z] INFO  [3460]  - [CMD-TailLogs/TailLogs] : Starting activity...
[2018-09-17T23:50:07.616Z] INFO  [3460]  - [CMD-TailLogs/TailLogs/TailLogs] : Starting activity...



-------------------------------------
/opt/python/log/sample-app.log
-------------------------------------




-------------------------------------
/var/log/eb-commandprocessor.log
-------------------------------------
[2018-09-17T23:29:07.266Z] DEBUG [2273]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||ManifestFileS3Key..
[2018-09-17T23:29:07.761Z] INFO  [2273]  : Finding latest manifest from bucket 'elasticbeanstalk-us-east-1-394343729102' with prefix 'resources/environments/e-2prvqhnsfz/_runtime/versions/manifest_'.
[2018-09-17T23:29:08.756Z] INFO  [2273]  : Found manifest with key 'resources/environments/e-2prvqhnsfz/_runtime/versions/manifest_1537226846106'.
[2018-09-17T23:29:08.795Z] INFO  [2273]  : Updated manifest cache: deployment ID 1 and serial 1.
[2018-09-17T23:29:08.795Z] DEBUG [2273]  : Loaded definition of Command CMD-PreInit.
[2018-09-17T23:29:08.795Z] INFO  [2273]  : Executing Initialization
[2018-09-17T23:29:08.796Z] INFO  [2273]  : Executing command: CMD-PreInit...
[2018-09-17T23:29:08.796Z] INFO  [2273]  : Executing command CMD-PreInit activities...
[2018-09-17T23:29:08.796Z] DEBUG [2273]  : Setting environment variables..
[2018-09-17T23:29:08.796Z] INFO  [2273]  : Running AddonsBefore for command CMD-PreInit...
[2018-09-17T23:29:15.208Z] DEBUG [2273]  : Running stages of Command CMD-PreInit from stage 0 to stage 0...
[2018-09-17T23:29:15.208Z] INFO  [2273]  : Running stage 0 of command CMD-PreInit...
[2018-09-17T23:29:15.209Z] DEBUG [2273]  : Loaded 2 actions for stage 0.
[2018-09-17T23:29:15.209Z] INFO  [2273]  : Running 1 of 2 actions: DownloadSourceBundle...
[2018-09-17T23:29:15.947Z] INFO  [2273]  : Running 2 of 2 actions: PreInitHook...
[2018-09-17T23:29:30.254Z] INFO  [2273]  : Running AddonsAfter for command CMD-PreInit...
[2018-09-17T23:29:30.255Z] INFO  [2273]  : Command CMD-PreInit succeeded!
[2018-09-17T23:29:30.255Z] INFO  [2273]  : Command processor returning results: 
{"status":"SUCCESS","api_version":"1.0","results":[{"status":"SUCCESS","msg":"","returncode":0,"events":[]}]}
[2018-09-17T23:30:08.330Z] DEBUG [2630]  : Reading config file: /etc/elasticbeanstalk/.aws-eb-stack.properties
[2018-09-17T23:30:08.331Z] DEBUG [2630]  : Checking if the command processor should execute...
[2018-09-17T23:30:08.333Z] DEBUG [2630]  : Checking whether the command is applicable to instance (i-055316f1bf6567d5d)..
[2018-09-17T23:30:08.333Z] INFO  [2630]  : Command is applicable to this instance (i-055316f1bf6567d5d)..
[2018-09-17T23:30:08.333Z] DEBUG [2630]  : Checking if the received command stage is valid..
[2018-09-17T23:30:08.333Z] INFO  [2630]  : No stage_num in command. Valid stage..
[2018-09-17T23:30:08.333Z] INFO  [2630]  : Received command CMD-Startup: {"execution_data"=>"{\"leader_election\":\"true\"}", "instance_ids"=>["i-055316f1bf6567d5d"], "command_name"=>"CMD-Startup", "api_version"=>"1.0", "resource_name"=>"AWSEBAutoScalingGroup", "request_id"=>"3627cff8-bad1-11e8-94d3-41166bc204f0"}
[2018-09-17T23:30:08.333Z] INFO  [2630]  : Command processor should execute command.
[2018-09-17T23:30:08.334Z] DEBUG [2630]  : Storing current stage..
[2018-09-17T23:30:08.334Z] DEBUG [2630]  : Stage_num does not exist. Not saving null stage. Returning..
[2018-09-17T23:30:08.334Z] DEBUG [2630]  : Reading config file: /etc/elasticbeanstalk/.aws-eb-stack.properties
[2018-09-17T23:30:08.334Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_ContainerConfigFileContent||commands..
[2018-09-17T23:30:08.335Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_API||_Commands..
[2018-09-17T23:30:08.336Z] INFO  [2630]  : Found enabled addons: ["logpublish", "logstreaming"].
[2018-09-17T23:30:08.339Z] INFO  [2630]  : Updating Command definition of addon logpublish.
[2018-09-17T23:30:08.339Z] INFO  [2630]  : Updating Command definition of addon logstreaming.
[2018-09-17T23:30:08.339Z] DEBUG [2630]  : Refreshing metadata...
[2018-09-17T23:30:09.084Z] DEBUG [2630]  : Refreshed environment metadata.
[2018-09-17T23:30:09.085Z] INFO  [2630]  : Recreated directory /opt/elasticbeanstalk/deploy/configuration/.
[2018-09-17T23:30:09.085Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_AppSourceUrlFileContent||url..
[2018-09-17T23:30:09.086Z] INFO  [2630]  : Created appsource url file at /opt/elasticbeanstalk/deploy/configuration/appsourceurl.
[2018-09-17T23:30:09.086Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_ContainerConfigFileContent..
[2018-09-17T23:30:09.090Z] INFO  [2630]  : Created container config file at /opt/elasticbeanstalk/deploy/configuration/containerconfiguration.
[2018-09-17T23:30:09.090Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_ContainerConfigFileContent||commands..
[2018-09-17T23:30:09.092Z] DEBUG [2630]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_API||_Commands..
[2018-09-17T23:30:09.093Z] INFO  [2630]  : Found enabled addons: ["logpublish", "logstreaming"].
[2018-09-17T23:30:09.095Z] INFO  [2630]  : Updating Command definition of addon logpublish.
[2018-09-17T23:30:09.095Z] INFO  [2630]  : Updating Command definition of addon logstreaming.
[2018-09-17T23:30:09.096Z] DEBUG [2630]  : Loaded definition of Command CMD-Startup.
[2018-09-17T23:30:09.097Z] INFO  [2630]  : Executing Application deployment
[2018-09-17T23:30:09.097Z] INFO  [2630]  : Executing command: CMD-Startup...
[2018-09-17T23:30:09.097Z] INFO  [2630]  : Executing command CMD-Startup activities...
[2018-09-17T23:30:09.097Z] DEBUG [2630]  : Setting environment variables..
[2018-09-17T23:30:09.098Z] INFO  [2630]  : Running AddonsBefore for command CMD-Startup...
[2018-09-17T23:30:09.349Z] DEBUG [2630]  : Running stages of Command CMD-Startup from stage 0 to stage 1...
[2018-09-17T23:30:09.349Z] INFO  [2630]  : Running stage 0 of command CMD-Startup...
[2018-09-17T23:30:09.349Z] INFO  [2630]  : Running leader election...
[2018-09-17T23:30:10.073Z] INFO  [2630]  : Instance is Leader.
[2018-09-17T23:30:10.073Z] DEBUG [2630]  : Loaded 7 actions for stage 0.
[2018-09-17T23:30:10.073Z] INFO  [2630]  : Running 1 of 7 actions: HealthdLogRotation...
[2018-09-17T23:30:10.086Z] INFO  [2630]  : Running 2 of 7 actions: HealthdHTTPDLogging...
[2018-09-17T23:30:10.087Z] INFO  [2630]  : Running 3 of 7 actions: HealthdNginxLogging...
[2018-09-17T23:30:10.087Z] INFO  [2630]  : Running 4 of 7 actions: EbExtensionPreBuild...
[2018-09-17T23:30:10.871Z] INFO  [2630]  : Running 5 of 7 actions: AppDeployPreHook...
[2018-09-17T23:30:15.637Z] INFO  [2630]  : Running 6 of 7 actions: EbExtensionPostBuild...
[2018-09-17T23:30:16.424Z] INFO  [2630]  : Running 7 of 7 actions: InfraCleanEbExtension...
[2018-09-17T23:30:16.426Z] INFO  [2630]  : Running stage 1 of command CMD-Startup...
[2018-09-17T23:30:16.426Z] DEBUG [2630]  : Loaded 3 actions for stage 1.
[2018-09-17T23:30:16.426Z] INFO  [2630]  : Running 1 of 3 actions: AppDeployEnactHook...
[2018-09-17T23:30:25.304Z] INFO  [2630]  : Running 2 of 3 actions: AppDeployPostHook...
[2018-09-17T23:30:25.304Z] INFO  [2630]  : Running 3 of 3 actions: PostInitHook...
[2018-09-17T23:30:25.315Z] INFO  [2630]  : Running AddonsAfter for command CMD-Startup...
[2018-09-17T23:30:25.484Z] INFO  [2630]  : Command CMD-Startup succeeded!
[2018-09-17T23:30:25.485Z] INFO  [2630]  : Command processor returning results: 
{"status":"SUCCESS","api_version":"1.0","results":[{"status":"SUCCESS","msg":"","returncode":0,"events":[]}]}
[2018-09-17T23:50:07.606Z] DEBUG [3460]  : Reading config file: /etc/elasticbeanstalk/.aws-eb-stack.properties
[2018-09-17T23:50:07.606Z] DEBUG [3460]  : Checking if the command processor should execute...
[2018-09-17T23:50:07.608Z] DEBUG [3460]  : Checking whether the command is applicable to instance (i-055316f1bf6567d5d)..
[2018-09-17T23:50:07.608Z] INFO  [3460]  : Command is applicable to this instance (i-055316f1bf6567d5d)..
[2018-09-17T23:50:07.608Z] DEBUG [3460]  : Checking if the received command stage is valid..
[2018-09-17T23:50:07.608Z] INFO  [3460]  : No stage_num in command. Valid stage..
[2018-09-17T23:50:07.608Z] INFO  [3460]  : Received command CMD-TailLogs: {"execution_data"=>"*", "instance_ids"=>["i-055316f1bf6567d5d"], "data"=>"66b7baa3-bad4-11e8-86eb-e5b79a448e72", "command_name"=>"CMD-TailLogs", "api_version"=>"1.0", "resource_name"=>"AWSEBAutoScalingGroup", "request_id"=>"66b7baa3-bad4-11e8-86eb-e5b79a448e72"}
[2018-09-17T23:50:07.609Z] INFO  [3460]  : Command processor should execute command.
[2018-09-17T23:50:07.609Z] DEBUG [3460]  : Storing current stage..
[2018-09-17T23:50:07.609Z] DEBUG [3460]  : Stage_num does not exist. Not saving null stage. Returning..
[2018-09-17T23:50:07.609Z] DEBUG [3460]  : Reading config file: /etc/elasticbeanstalk/.aws-eb-stack.properties
[2018-09-17T23:50:07.609Z] DEBUG [3460]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_ContainerConfigFileContent||commands..
[2018-09-17T23:50:07.610Z] DEBUG [3460]  : Retrieving metadata for key: AWS::ElasticBeanstalk::Ext||_API||_Commands..
[2018-09-17T23:50:07.611Z] INFO  [3460]  : Found enabled addons: ["logpublish", "logstreaming"].
[2018-09-17T23:50:07.614Z] INFO  [3460]  : Updating Command definition of addon logpublish.
[2018-09-17T23:50:07.614Z] INFO  [3460]  : Updating Command definition of addon logstreaming.
[2018-09-17T23:50:07.614Z] DEBUG [3460]  : Loaded definition of Command CMD-TailLogs.
[2018-09-17T23:50:07.614Z] INFO  [3460]  : Executing CMD-TailLogs
[2018-09-17T23:50:07.615Z] INFO  [3460]  : Executing command: CMD-TailLogs...
[2018-09-17T23:50:07.615Z] INFO  [3460]  : Executing command CMD-TailLogs activities...
[2018-09-17T23:50:07.615Z] DEBUG [3460]  : Setting environment variables..
[2018-09-17T23:50:07.615Z] INFO  [3460]  : Running AddonsBefore for command CMD-TailLogs...
[2018-09-17T23:50:07.615Z] DEBUG [3460]  : Running stages of Command CMD-TailLogs from stage 0 to stage 0...
[2018-09-17T23:50:07.615Z] INFO  [3460]  : Running stage 0 of command CMD-TailLogs...
[2018-09-17T23:50:07.616Z] DEBUG [3460]  : Loaded 1 actions for stage 0.
[2018-09-17T23:50:07.616Z] INFO  [3460]  : Running 1 of 1 actions: TailLogs...


