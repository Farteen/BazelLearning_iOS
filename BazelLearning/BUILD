objc_library(
	name = "BazelTestingClasses",
	srcs = [
			"BazelLearning/AppDelegate.m",
			"BazelLearning/ViewController.m",
	],
	hdrs = glob(["BazelLearning/*.h"]),
	xibs = glob(["BazelLearning/*.xib"]),
	)

objc_binary(
	name = "BazelTestingBinary",
	srcs = [
	"BazelLearning/main.m",
	],
	deps = [
		":BazelTestingClasses",
	],
	)

ios_application(
	name = "BazelTestingApplication",
	binary = ":BazelTestingBinary",
	infoplist = "BazelLearning/Info.plist",
	)