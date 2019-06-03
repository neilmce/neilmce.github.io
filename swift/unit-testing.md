# Unit Testing

This is based on Apple's [XCTest framework](https://developer.apple.com/documentation/xctest),
which can be used to test synchronous & asynchronous code for correctness & for performance.
See [examples](https://developer.apple.com/documentation/xctest/defining_test_cases_and_test_methods).

A unit test class has the same basic form as a JUnit class:
```swift
import XCTest
@testable import UnitTestSpike

class UnitTestSpikeTests: XCTestCase {
  override func setUp() {}
  override func tearDown() {}
  func testMethod1() {}
  func testMethod2() {}
}
```

Assertions can be made as follows:
```swift
XCTAssert(list.isEmpty)
XCTAssertEqual(list.count, 10)
```

Performance tests are made as follows:
```swift
func testPerformanceExample() {
  self.measure {
    // Put the code you want to measure the time of here.
  }
}
```
