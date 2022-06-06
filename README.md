# extended Cyber Analytics Repository Model

The eCAR data model is used to describe host-based behavior, and is based on MITRE's Cyber Analytics Model using a similar data tuple of Object-Action-Properties to describe activity. It is extended as a process-oriented model by the elevation of process information as top-level data features, attribution with object/parent-actor UUIDs, and addition of host identity. 

The specification doesn't declare valid Object-Action pairings, but in practice only certain elements will make sense. It is possible for differnt event sources using eCAR to select similar but different object-action pairs for the same general activity.

eCAR Objects include:
 * driver - system drivers
 * file - file objects and streams
 * flow - network flows and ports
 * module - DLLs and other library loads
 * process - process activity
 * registry - Windows registry hive activity
 * service - system service activity
 * thread - threads activitvy
 * user_Session - user and service logins 
 * host - system start and notice activity
 * log - OS logging activity 
 * WMI - Windows management system activity
 * sensor - activity related to endpoint sensor generating the eCAR events
 * task - 
 * token - authentication 
 * dns - DNS activity
 * shell - 
 * otherobj - catchall for uncategorized activities
 
eCAR Actions include:   
| add | create | clear | close | delete |  
| edit | end | load| message | modify |  
| open | pause | read | remote_create | remove |  
| start | stop | suspend | terminate | timestomp |   
| unload | write | interactive | local | login |   
| logout | rdp | reconnect | rempte | unlock |    
| heartbeat | info | invoke | request| response |    
| operation | rename | receive | grant | renew |  
| command | otheract |   |   |    |  


