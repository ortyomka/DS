# DS lab9

### rs.conf()
```
{
	"_id" : "rs0",
	"version" : 1,
	"protocolVersion" : NumberLong(1),
	"writeConcernMajorityJournalDefault" : true,
	"members" : [
		{
			"_id" : 0,
			"host" : "v1:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 1,
			"host" : "v2:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 2,
			"host" : "v3:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		}
	],
	"settings" : {
		"chainingAllowed" : true,
		"heartbeatIntervalMillis" : 2000,
		"heartbeatTimeoutSecs" : 10,
		"electionTimeoutMillis" : 10000,
		"catchUpTimeoutMillis" : -1,
		"catchUpTakeoverDelayMillis" : 30000,
		"getLastErrorModes" : {
			
		},
		"getLastErrorDefaults" : {
			"w" : 1,
			"wtimeout" : 0
		},
		"replicaSetId" : ObjectId("5db92ba2670b855eca03d0f0")
	}
}
```

### rs.status()
```
{
	"set" : "rs0",
	"date" : ISODate("2019-10-30T06:40:01.753Z"),
	"myState" : 1,
	"term" : NumberLong(1),
	"syncingTo" : "",
	"syncSourceHost" : "",
	"syncSourceId" : -1,
	"heartbeatIntervalMillis" : NumberLong(2000),
	"majorityVoteCount" : 2,
	"writeMajorityCount" : 2,
	"optimes" : {
		"lastCommittedOpTime" : {
			"ts" : Timestamp(1572417600, 1),
			"t" : NumberLong(1)
		},
		"lastCommittedWallTime" : ISODate("2019-10-30T06:40:00.115Z"),
		"readConcernMajorityOpTime" : {
			"ts" : Timestamp(1572417600, 1),
			"t" : NumberLong(1)
		},
		"readConcernMajorityWallTime" : ISODate("2019-10-30T06:40:00.115Z"),
		"appliedOpTime" : {
			"ts" : Timestamp(1572417600, 1),
			"t" : NumberLong(1)
		},
		"durableOpTime" : {
			"ts" : Timestamp(1572417600, 1),
			"t" : NumberLong(1)
		},
		"lastAppliedWallTime" : ISODate("2019-10-30T06:40:00.115Z"),
		"lastDurableWallTime" : ISODate("2019-10-30T06:40:00.115Z")
	},
	"lastStableRecoveryTimestamp" : Timestamp(1572417570, 1),
	"lastStableCheckpointTimestamp" : Timestamp(1572417570, 1),
	"electionCandidateMetrics" : {
		"lastElectionReason" : "electionTimeout",
		"lastElectionDate" : ISODate("2019-10-30T06:20:29.374Z"),
		"termAtElection" : NumberLong(1),
		"lastCommittedOpTimeAtElection" : {
			"ts" : Timestamp(0, 0),
			"t" : NumberLong(-1)
		},
		"lastSeenOpTimeAtElection" : {
			"ts" : Timestamp(1572416419, 1),
			"t" : NumberLong(-1)
		},
		"numVotesNeeded" : 2,
		"priorityAtElection" : 1,
		"electionTimeoutMillis" : NumberLong(10000),
		"numCatchUpOps" : NumberLong(27017),
		"newTermStartDate" : ISODate("2019-10-30T06:20:30.082Z"),
		"wMajorityWriteAvailabilityDate" : ISODate("2019-10-30T06:20:30.952Z")
	},
	"members" : [
		{
			"_id" : 0,
			"name" : "v1:27017",
			"ip" : "172.31.37.187",
			"health" : 1,
			"state" : 1,
			"stateStr" : "PRIMARY",
			"uptime" : 1365,
			"optime" : {
				"ts" : Timestamp(1572417600, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-30T06:40:00Z"),
			"syncingTo" : "",
			"syncSourceHost" : "",
			"syncSourceId" : -1,
			"infoMessage" : "",
			"electionTime" : Timestamp(1572416429, 1),
			"electionDate" : ISODate("2019-10-30T06:20:29Z"),
			"configVersion" : 1,
			"self" : true,
			"lastHeartbeatMessage" : ""
		},
		{
			"_id" : 1,
			"name" : "v2:27017",
			"ip" : "172.31.33.46",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 1182,
			"optime" : {
				"ts" : Timestamp(1572417600, 1),
				"t" : NumberLong(1)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572417600, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-30T06:40:00Z"),
			"optimeDurableDate" : ISODate("2019-10-30T06:40:00Z"),
			"lastHeartbeat" : ISODate("2019-10-30T06:40:01.700Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-30T06:40:01Z"),
			"pingMs" : NumberLong(0),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "v1:27017",
			"syncSourceHost" : "v1:27017",
			"syncSourceId" : 0,
			"infoMessage" : "",
			"configVersion" : 1
		},
		{
			"_id" : 2,
			"name" : "v3:27017",
			"ip" : "172.31.39.231",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 1182,
			"optime" : {
				"ts" : Timestamp(1572417600, 1),
				"t" : NumberLong(1)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572417600, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-30T06:40:00Z"),
			"optimeDurableDate" : ISODate("2019-10-30T06:40:00Z"),
			"lastHeartbeat" : ISODate("2019-10-30T06:40:01.700Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-30T06:40:01.135Z"),
			"pingMs" : NumberLong(0),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "v1:27017",
			"syncSourceHost" : "v1:27017",
			"syncSourceId" : 0,
			"infoMessage" : "",
			"configVersion" : 1
		}
	],
	"ok" : 1,
	"$clusterTime" : {
		"clusterTime" : Timestamp(1572417600, 1),
		"signature" : {
			"hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
			"keyId" : NumberLong(0)
		}
	},
	"operationTime" : Timestamp(1572417600, 1)
}
```
### app
![](https://i.imgur.com/GevxCMe.png)

---

### rs.conf()
```
{
	"_id" : "rs0",
	"version" : 1,
	"protocolVersion" : NumberLong(1),
	"writeConcernMajorityJournalDefault" : true,
	"members" : [
		{
			"_id" : 0,
			"host" : "v1:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 1,
			"host" : "v2:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 2,
			"host" : "v3:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {
				
			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		}
	],
	"settings" : {
		"chainingAllowed" : true,
		"heartbeatIntervalMillis" : 2000,
		"heartbeatTimeoutSecs" : 10,
		"electionTimeoutMillis" : 10000,
		"catchUpTimeoutMillis" : -1,
		"catchUpTakeoverDelayMillis" : 30000,
		"getLastErrorModes" : {
			
		},
		"getLastErrorDefaults" : {
			"w" : 1,
			"wtimeout" : 0
		},
		"replicaSetId" : ObjectId("5db92ba2670b855eca03d0f0")
	}
}
```
### rs.status()
```
{
	"set" : "rs0",
	"date" : ISODate("2019-10-30T06:50:36.504Z"),
	"myState" : 1,
	"term" : NumberLong(2),
	"syncingTo" : "",
	"syncSourceHost" : "",
	"syncSourceId" : -1,
	"heartbeatIntervalMillis" : NumberLong(2000),
	"majorityVoteCount" : 2,
	"writeMajorityCount" : 2,
	"optimes" : {
		"lastCommittedOpTime" : {
			"ts" : Timestamp(1572418228, 1),
			"t" : NumberLong(2)
		},
		"lastCommittedWallTime" : ISODate("2019-10-30T06:50:28.156Z"),
		"readConcernMajorityOpTime" : {
			"ts" : Timestamp(1572418228, 1),
			"t" : NumberLong(2)
		},
		"readConcernMajorityWallTime" : ISODate("2019-10-30T06:50:28.156Z"),
		"appliedOpTime" : {
			"ts" : Timestamp(1572418228, 1),
			"t" : NumberLong(2)
		},
		"durableOpTime" : {
			"ts" : Timestamp(1572418228, 1),
			"t" : NumberLong(2)
		},
		"lastAppliedWallTime" : ISODate("2019-10-30T06:50:28.156Z"),
		"lastDurableWallTime" : ISODate("2019-10-30T06:50:28.156Z")
	},
	"lastStableRecoveryTimestamp" : Timestamp(1572418228, 1),
	"lastStableCheckpointTimestamp" : Timestamp(1572418228, 1),
	"electionCandidateMetrics" : {
		"lastElectionReason" : "stepUpRequestSkipDryRun",
		"lastElectionDate" : ISODate("2019-10-30T06:42:47.705Z"),
		"termAtElection" : NumberLong(2),
		"lastCommittedOpTimeAtElection" : {
			"ts" : Timestamp(1572417760, 1),
			"t" : NumberLong(1)
		},
		"lastSeenOpTimeAtElection" : {
			"ts" : Timestamp(1572417760, 1),
			"t" : NumberLong(1)
		},
		"numVotesNeeded" : 2,
		"priorityAtElection" : 1,
		"electionTimeoutMillis" : NumberLong(10000),
		"priorPrimaryMemberId" : 0,
		"numCatchUpOps" : NumberLong(27017),
		"newTermStartDate" : ISODate("2019-10-30T06:42:48.144Z"),
		"wMajorityWriteAvailabilityDate" : ISODate("2019-10-30T06:42:49.276Z")
	},
	"members" : [
		{
			"_id" : 0,
			"name" : "v1:27017",
			"ip" : "172.31.37.187",
			"health" : 0,
			"state" : 8,
			"stateStr" : "(not reachable/healthy)",
			"uptime" : 0,
			"optime" : {
				"ts" : Timestamp(0, 0),
				"t" : NumberLong(-1)
			},
			"optimeDurable" : {
				"ts" : Timestamp(0, 0),
				"t" : NumberLong(-1)
			},
			"optimeDate" : ISODate("1970-01-01T00:00:00Z"),
			"optimeDurableDate" : ISODate("1970-01-01T00:00:00Z"),
			"lastHeartbeat" : ISODate("2019-10-30T06:50:35.309Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-30T06:42:47.760Z"),
			"pingMs" : NumberLong(5),
			"lastHeartbeatMessage" : "Error connecting to v1:27017 (172.31.37.187:27017) :: caused by :: No route to host",
			"syncingTo" : "",
			"syncSourceHost" : "",
			"syncSourceId" : -1,
			"infoMessage" : "",
			"configVersion" : -1
		},
		{
			"_id" : 1,
			"name" : "v2:27017",
			"ip" : "172.31.33.46",
			"health" : 1,
			"state" : 1,
			"stateStr" : "PRIMARY",
			"uptime" : 1937,
			"optime" : {
				"ts" : Timestamp(1572418228, 1),
				"t" : NumberLong(2)
			},
			"optimeDate" : ISODate("2019-10-30T06:50:28Z"),
			"syncingTo" : "",
			"syncSourceHost" : "",
			"syncSourceId" : -1,
			"infoMessage" : "",
			"electionTime" : Timestamp(1572417767, 1),
			"electionDate" : ISODate("2019-10-30T06:42:47Z"),
			"configVersion" : 1,
			"self" : true,
			"lastHeartbeatMessage" : ""
		},
		{
			"_id" : 2,
			"name" : "v3:27017",
			"ip" : "172.31.39.231",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 1817,
			"optime" : {
				"ts" : Timestamp(1572418228, 1),
				"t" : NumberLong(2)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572418228, 1),
				"t" : NumberLong(2)
			},
			"optimeDate" : ISODate("2019-10-30T06:50:28Z"),
			"optimeDurableDate" : ISODate("2019-10-30T06:50:28Z"),
			"lastHeartbeat" : ISODate("2019-10-30T06:50:35.781Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-30T06:50:35.369Z"),
			"pingMs" : NumberLong(0),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "v2:27017",
			"syncSourceHost" : "v2:27017",
			"syncSourceId" : 1,
			"infoMessage" : "",
			"configVersion" : 1
		}
	],
	"ok" : 1,
	"$clusterTime" : {
		"clusterTime" : Timestamp(1572418228, 1),
		"signature" : {
			"hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
			"keyId" : NumberLong(0)
		}
	},
	"operationTime" : Timestamp(1572418228, 1)
}
```
### app
![](https://i.imgur.com/yyeETNv.png)

Code from here [original](https://github.com/amkurian/simple-chat)
Modified by me