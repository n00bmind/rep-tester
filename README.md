# rep-tester
Repetition Tester in jai

Inspired by https://www.computerenhance.com/p/repetition-testing


## Usage

```
    tester: RepetitionTester;
    // Optionally pass a total byte count, to get a bytes-per-second figure
    NewTestWave( *tester, totalByteCount );

    while BeginTestCycle( *tester )
    {
        BeginTime( *tester );

        // Execute one test cycle
        DoTest();

        EndTime( *tester );
        // Optionally pass how many bytes this one cycle completed
        CountBytes( *tester, cycleByteCount );
    }
```
