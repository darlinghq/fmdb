project(fmdb)

set(sources
	src/fmdb/FMDatabaseAdditions.m
	src/fmdb/FMDatabase.m
	src/fmdb/FMDatabasePool.m
	src/fmdb/FMDatabaseQueue.m
	src/fmdb/FMResultSet.m
)

add_framework(FMDB
	FAT
	CURRENT_VERSION
	PRIVATE
	VERSION "A"

	SOURCES
		${sources}

	DEPENDENCIES
		system
		Foundation
		sqlite3
)


