# ArcHarp
Head direction .
 <$ go test -v -timeout 10s -run ^TestKeeperTestSuite/TestCreateGroupWithLotsOfMembers$ ./x/group/keeper/...> 
=== RUN   TestKeeperTestSuite
=== RUN   TestKeeperTestSuite/TestCreateGroupWithLotsOfMembers
    keeper_test.go:115: group 2 created with 50 members
    keeper_test.go:120: got 50 members from group 2
    keeper_test.go:115: group 3 created with 51 members
    keeper_test.go:120: got 51 members from group 3
    keeper_test.go:115: group 4 created with 52 members
    keeper_test.go:120: got 52 members from group 4
    keeper_test.go:115: group 5 created with 53 members
    keeper_test.go:120: got 53 members from group 5
    keeper_test.go:115: group 6 created with 54 members
    keeper_test.go:120: got 54 members from group 6
    keeper_test.go:115: group 7 created with 55 members
    keeper_test.go:120: got 55 members from group 7
    keeper_test.go:115: group 8 created with 56 members
    keeper_test.go:120: got 56 members from group 8
    keeper_test.go:115: group 9 created with 57 members
    keeper_test.go:120: got 57 members from group 9
    keeper_test.go:115: group 10 created with 58 members
    keeper_test.go:120: got 58 members from group 10
    keeper_test.go:115: group 11 created with 59 members
    keeper_test.go:120: got 59 members from group 11
    keeper_test.go:115: group 12 created with 60 members
    keeper_test.go:120: got 60 members from group 12
    keeper_test.go:115: group 13 created with 61 members
    keeper_test.go:120: got 61 members from group 13
    keeper_test.go:115: group 14 created with 62 members
    keeper_test.go:120: got 62 members from group 14
    keeper_test.go:115: group 15 created with 63 members
    keeper_test.go:120: got 63 members from group 15
    keeper_test.go:115: group 16 created with 64 members
    keeper_test.go:120: got 64 members from group 16
    keeper_test.go:115: group 17 created with 65 members
    keeper_test.go:120: got 65 members from group 17
    keeper_test.go:115: group 18 created with 66 members
    keeper_test.go:120: got 66 members from group 18
    keeper_test.go:115: group 19 created with 67 members
panic: test timed out after 10s

goroutine 26 [running]:
testing.(*M).startAlarm.func1()
        /usr/lib/go/src/testing/testing.go:2029 +0x8e
created by time.goFunc
        /usr/lib/go/src/time/sleep.go:176 +0x32

goroutine 1 [chan receive]:
testing.(*T).Run(0xc00097a4e0, {0x1f4858b?, 0x522ee5?}, 0x26222b0)
        /usr/lib/go/src/testing/testing.go:1487 +0x37a
testing.runTests.func1(0xc0005c4420?)
        /usr/lib/go/src/testing/testing.go:1839 +0x6e
testing.tRunner(0xc00097a4e0, 0xc000b3fcd8)
        /usr/lib/go/src/testing/testing.go:1439 +0x102
testing.runTests(0xc0008181e0?, {0x38e2640, 0x4, 0x4}, {0x7f6610334108?, 0x40?, 0x3907180?})
        /usr/lib/go/src/testing/testing.go:1837 +0x457
testing.(*M).Run(0xc0008181e0)
        /usr/lib/go/src/testing/testing.go:1719 +0x5d9
main.main()
        _testmain.go:55 +0x1aa

goroutine 42 [IO wait]:
internal/poll.runtime_pollWait(0x7f65e8532100, 0x72)
        /usr/lib/go/src/runtime/netpoll.go:302 +0x89
internal/poll.(*pollDesc).wait(0xc00013c400?, 0xc0005404d0?, 0x0)
        /usr/lib/go/src/internal/poll/fd_poll_runtime.go:83 +0x32
internal/poll.(*pollDesc).waitRead(...)
        /usr/lib/go/src/internal/poll/fd_poll_runtime.go:88
internal/poll.(*FD).ReadMsg(0xc00013c400, {0xc0005404d0, 0x10, 0x10}, {0xc000590020, 0x1000, 0x1000}, 0x4173af?)
        /usr/lib/go/src/internal/poll/fd_unix.go:304 +0x31c
net.(*netFD).readMsg(0xc00013c400, {0xc0005404d0?, 0x7f661033d668?, 0x0?}, {0xc000590020?, 0x418fe5?, 0x393adc0?}, 0xc000513d08?)
        /usr/lib/go/src/net/fd_posix.go:78 +0x37
net.(*UnixConn).readMsg(0xc0005226c0, {0xc0005404d0?, 0xc000513d80?, 0x40f645?}, {0xc000590020?, 0xb?, 0x7f65e9a22fff?})
        /usr/lib/go/src/net/unixsock_posix.go:115 +0x4f
net.(*UnixConn).ReadMsgUnix(0xc0005226c0, {0xc0005404d0?, 0xc000513df8?, 0x40f645?}, {0xc000590020?, 0x0?, 0x0?})
        /usr/lib/go/src/net/unixsock.go:143 +0x3c
github.com/godbus/dbus.(*oobReader).Read(0xc000590000, {0xc0005404d0?, 0xc000513e20?, 0x40f9a7?})
        /home/user/go/pkg/mod/github.com/godbus/dbus@v0.0.0-20190726142602-4481cbc300e2/transport_unix.go:21 +0x45
io.ReadAtLeast({0x293f8c0, 0xc000590000}, {0xc0005404d0, 0x10, 0x10}, 0x10)
        /usr/lib/go/src/io/io.go:331 +0x9a
io.ReadFull(...)
        /usr/lib/go/src/io/io.go:350
github.com/godbus/dbus.(*unixTransport).ReadMessage(0xc000531068)
        /home/user/go/pkg/mod/github.com/godbus/dbus@v0.0.0-20190726142602-4481cbc300e2/transport_unix.go:91 +0x11e
github.com/godbus/dbus.(*Conn).inWorker(0xc0000f2d80)
        /home/user/go/pkg/mod/github.com/godbus/dbus@v0.0.0-20190726142602-4481cbc300e2/conn.go:294 +0x3b
created by github.com/godbus/dbus.(*Conn).Auth
        /home/user/go/pkg/mod/github.com/godbus/dbus@v0.0.0-20190726142602-4481cbc300e2/auth.go:118 +0x9ed

goroutine 55 [select]:
github.com/desertbit/timer.timerRoutine()
        /home/user/go/pkg/mod/github.com/desertbit/timer@v0.0.0-20180107155436-c41aec40b27f/timers.go:119 +0xba
created by github.com/desertbit/timer.init.0
        /home/user/go/pkg/mod/github.com/desertbit/timer@v0.0.0-20180107155436-c41aec40b27f/timers.go:15 +0x25

goroutine 10 [select]:
go.opencensus.io/stats/view.(*worker).start(0xc00013c880)
        /home/user/go/pkg/mod/go.opencensus.io@v0.23.0/stats/view/worker.go:276 +0xad
created by go.opencensus.io/stats/view.init.0
        /home/user/go/pkg/mod/go.opencensus.io@v0.23.0/stats/view/worker.go:34 +0x8d

goroutine 11 [chan receive]:
testing.(*T).Run(0xc00097a680, {0x1b86dea?, 0xc00097a680?}, 0xc000b65290)
        /usr/lib/go/src/testing/testing.go:1487 +0x37a
github.com/stretchr/testify/suite.runTests({0x2971988, 0xc00097a680}, {0xc0002f0600?, 0x14, 0x20})
        /home/user/go/pkg/mod/github.com/stretchr/testify@v1.7.1/suite/suite.go:203 +0x128
github.com/stretchr/testify/suite.Run(0xc00097a680, {0x2945c10, 0xc000580c00})
        /home/user/go/pkg/mod/github.com/stretchr/testify@v1.7.1/suite/suite.go:176 +0x6e5
github.com/cosmos/cosmos-sdk/x/group/keeper_test.TestKeeperTestSuite(0x0?)
        /home/user/workspace/cosmos/cosmos-sdk/x/group/keeper/keeper_test.go:85 +0x39
testing.tRunner(0xc00097a680, 0x26222b0)
        /usr/lib/go/src/testing/testing.go:1439 +0x102
created by testing.(*T).Run
        /usr/lib/go/src/testing/testing.go:1486 +0x35f

goroutine 12 [semacquire]:
sync.runtime_SemacquireMutex(0x203000?, 0x0?, 0xc000f157c8?)
        /usr/lib/go/src/runtime/sema.go:71 +0x25
sync.(*RWMutex).Lock(0x0?)
        /usr/lib/go/src/sync/rwmutex.go:144 +0x71
github.com/tendermint/tm-db.(*MemDB).Set(0xc000b4fbe0, {0xc000ac9bc0, 0x1e, 0x20}, {0xc00084d3b0, 0x44, 0x44})
        /home/user/go/pkg/mod/github.com/tendermint/tm-db@v0.6.6/memdb.go:100 +0x85
github.com/cosmos/cosmos-sdk/store/cachekv.(*Store).clearUnsortedCacheSubset(0xc0009f2700, {0xc000cabbb0?, 0x2, 0x2}, 0x1)
        /home/user/workspace/cosmos/cosmos-sdk/store/cachekv/store.go:359 +0x165
github.com/cosmos/cosmos-sdk/store/cachekv.(*Store).dirtyItems(0xc0009f2700, {0xc000ac9b40, 0x1e, 0x1e}, {0xc000ac9ba0, 0x1e, 0x1e})
        /home/user/workspace/cosmos/cosmos-sdk/store/cachekv/store.go:331 +0x52b
github.com/cosmos/cosmos-sdk/store/cachekv.(*Store).iterator(0xc0009f2700, {0xc000ac9b40, 0x1e, 0x1e}, {0xc000ac9ba0, 0x1e, 0x1e}, 0x1)
        /home/user/workspace/cosmos/cosmos-sdk/store/cachekv/store.go:190 +0x17e
github.com/cosmos/cosmos-sdk/store/cachekv.(*Store).Iterator(0xc000e0ac40?, {0xc000ac9b40?, 0xc000f15b28?, 0x0?}, {0xc000ac9ba0?, 0x1?, 0x40f645?})
        /home/user/workspace/cosmos/cosmos-sdk/store/cachekv/store.go:170 +0x29
github.com/cosmos/cosmos-sdk/store/gaskv.(*Store).iterator(0xc0004143c0, {0xc000ac9b40?, 0x0?, 0xc000f15b00?}, {0xc000ac9ba0?, 0x2?, 0x1?}, 0xa0?)
        /home/user/workspace/cosmos/cosmos-sdk/store/gaskv/store.go:103 +0x56
github.com/cosmos/cosmos-sdk/store/gaskv.(*Store).Iterator(0xc000420800?, {0xc000ac9b40?, 0x25?, 0xc0006172cc?}, {0xc000ac9ba0?, 0x40f645?, 0xc0003d09f0?})
        /home/user/workspace/cosmos/cosmos-sdk/store/gaskv/store.go:74 +0x29
github.com/cosmos/cosmos-sdk/store/prefix.Store.Iterator({{0x2966738, 0xc0004143c0}, {0xc0006172cc, 0x2, 0x2}}, {0xc0003d09c9, 0x1c, 0x27}, {0xc000ac99e0, 0x1c, ...})
        /home/user/workspace/cosmos/cosmos-sdk/store/prefix/store.go:101 +0x239
github.com/cosmos/cosmos-sdk/x/group/internal/orm.NewTypeSafeRowGetter.func1({0x2966738, 0xc0004143c0}, {0xc0003d09c9, 0x1c, 0x27}, {0x29643f8, 0xc000cabb90})
        /home/user/workspace/cosmos/cosmos-sdk/x/group/internal/orm/types.go:116 +0x2f4
github.com/cosmos/cosmos-sdk/x/group/internal/orm.indexIterator.LoadNext({{0x2966738, 0xc0004143c0}, 0xc0009fb1a0, {0x2960fc0, 0xc0004145a0}, {0x1c0a0c0, 0x388eb20}}, {0x29643f8, 0xc000cabb90})
        /home/user/workspace/cosmos/cosmos-sdk/x/group/internal/orm/index.go:253 +0x106
github.com/cosmos/cosmos-sdk/x/group/internal/orm.Paginate({0x2947948?, 0xc000e0ac40}, 0x295a2b0?, {0x1bb2580?, 0xc00080b8f0?})
        /home/user/workspace/cosmos/cosmos-sdk/x/group/internal/orm/iterator.go:180 +0x42a
github.com/cosmos/cosmos-sdk/x/group/keeper.Keeper.GroupMembers({{0x2945a08, 0xc0009ee170}, {0x295a2b0, 0xc000025900}, {0xc000239200, {0x1}}, {0x295df20, 0xc0009f31c0}, {0xc000239260}, {0x295df20, ...}, ...}, ...)
        /home/user/workspace/cosmos/cosmos-sdk/x/group/keeper/grpc_query.go:63 +0x31f
github.com/cosmos/cosmos-sdk/x/group/keeper_test.(*TestSuite).createGroupAndGetMembers(0xc000580c00, 0x43)
        /home/user/workspace/cosmos/cosmos-sdk/x/group/keeper/keeper_test.go:117 +0x5a5
github.com/cosmos/cosmos-sdk/x/group/keeper_test.(*TestSuite).TestCreateGroupWithLotsOfMembers(0xc000580c00)
        /home/user/workspace/cosmos/cosmos-sdk/x/group/keeper/keeper_test.go:95 +0x97
reflect.Value.call({0xc0007974a0?, 0xc0005610e8?, 0x2965ef0?}, {0x1f3163e, 0x4}, {0xc000a0fe70, 0x1, 0xc000a0fd80?})
        /usr/lib/go/src/reflect/value.go:556 +0x845
reflect.Value.Call({0xc0007974a0?, 0xc0005610e8?, 0xc000580c00?}, {0xc000a0fe70, 0x1, 0x1})
        /usr/lib/go/src/reflect/value.go:339 +0xbf
github.com/stretchr/testify/suite.Run.func1(0xc00097ab60)
        /home/user/go/pkg/mod/github.com/stretchr/testify@v1.7.1/suite/suite.go:158 +0x4b6
testing.tRunner(0xc00097ab60, 0xc000b65290)
        /usr/lib/go/src/testing/testing.go:1439 +0x102
created by testing.(*T).Run
        /usr/lib/go/src/testing/testing.go:1486 +0x35f

goroutine 3302 [select]:
github.com/tendermint/tm-db.newMemDBIteratorMtxChoice.func1.1({0x2940340?, 0xc0003e7530})
        /home/user/go/pkg/mod/github.com/tendermint/tm-db@v0.6.6/memdb_iterator.go:67 +0x18e
github.com/google/btree.(*node).iterate(0xc000e0abc0, 0x1, {0x2940340, 0xc0003e7560}, {0x2940340, 0xc0003e75c0}, 0x1, 0x1, 0xc00009af98)
        /home/user/go/pkg/mod/github.com/google/btree@v1.0.1/btree.go:524 +0x322
github.com/google/btree.(*node).iterate(0xc0003ce580, 0x1, {0x2940340, 0xc0003e7560}, {0x2940340, 0xc0003e75c0}, 0x1, 0x0, 0xc00009af98)
        /home/user/go/pkg/mod/github.com/google/btree@v1.0.1/btree.go:529 +0x3b3
github.com/google/btree.(*BTree).AscendRange(...)
        /home/user/go/pkg/mod/github.com/google/btree@v1.0.1/btree.go:750
github.com/tendermint/tm-db.newMemDBIteratorMtxChoice.func1()
        /home/user/go/pkg/mod/github.com/tendermint/tm-db@v0.6.6/memdb_iterator.go:83 +0x2ee
created by github.com/tendermint/tm-db.newMemDBIteratorMtxChoice
        /home/user/go/pkg/mod/github.com/tendermint/tm-db@v0.6.6/memdb_iterator.go:48 +0x2cf
FAIL    github.com/cosmos/cosmos-sdk/x/group/keeper     10.053s
True 
bitcoincash:qzqqq8yrppj9nz849t3307vc3dmnp4uafqsfu0wqyd?amount=0.002&label=Bitcoin%20Cash%20Notary&message=Proof%20of%20document%203ed5709853b1a56ca133d9ae16d04acd65f91081cc076c9c4cb29b63a1bc42b4
bitcoincash:qrezymekj8r0nk4fq87nxat7qshs05axrgpjkam738![received_1988790021519707](https://github.com/Aroc902322/ArcHarp/assets/131215639/94260cb7-2e2d-4ec3-8350-119087fca912)
![received_1301457633908812](https://github.com/Aroc902322/ArcHarp/assets/131215639/825a6d56-b36c-4b2c-9c92-1a3651f0c3c0)
