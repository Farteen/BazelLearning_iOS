objc_library(
	name = "BazelTestingClasses",
	srcs = [
			"BazelLearning/BazelLearning/AppDelegate.m",
			"BazelLearning/BazelLearning/ViewController.m",
	],
	hdrs = glob(["BazelLearning/BazelLearning/*.h"]),
	xibs = glob(["BazelLearning/BazelLearning/*.xib"]),
	)

objc_binary(
	name = "BazelTestingBinary",
	srcs = [
	"BazelLearning/BazelLearning/main.m",
	],
	deps = [
		":BazelTestingClasses",
	],
	)

ios_application(
	name = "BazelTestingApplication",
	binary = ":BazelTestingBinary",
	infoplist = "BazelLearning/BazelLearning/Info.plist",
	)