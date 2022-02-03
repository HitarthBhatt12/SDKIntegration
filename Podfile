# Uncomment the next line to define a global platform for your project
source 'https://github.com/CocoaPods/Specs.git'

target 'Runnning-Buddy' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
platform :ios, '13.0'

use_frameworks!
inhibit_all_warnings!

pod 'SDWebImage', '5.12.1'
pod 'AWSCore', '2.19.1'
pod 'AWSS3', '2.19.1'
pod 'HNKGooglePlacesAutocomplete', '~> 1.1'
pod 'Mapbox-iOS-SDK', '~> 6.3.0'
pod 'Firebase’
pod 'Firebase/Auth' #,'~> 4.4.1'
pod 'Firebase/Database'
pod 'THLabel'
pod 'Permission/Camera'
pod 'Permission/Notifications'
pod 'Permission/Bluetooth'
pod 'Permission/Contacts'
pod 'Permission/Location'
pod 'Permission/Microphone'
pod 'Permission/Motion'
pod 'Permission/Photos'
pod 'Permission/Reminders'
pod 'Permission/MediaLibrary'
pod 'Permission/Siri'
pod 'APNGKit', '~> 1.1.0'
pod 'Alamofire', '~> 4.7.3'
pod 'FMDB'
pod 'TPKeyboardAvoiding'
pod 'iCarousel'
pod 'MASAttributes', '~> 1.0'
pod 'Bagel'
pod 'DynamicBlurView', '~> 4.0.0'
pod 'Signals', '6.1.0'
end


target 'ARunnning-BuddyWatch' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  platform :watchos, '7.0'
  pod 'Mapbox-iOS-SDK', '~> 6.3.0' "Crash is here"


end

target 'Runnning-Buddy Extension' do
  #pod 'Firebase/Auth'
  #pod 'Firebase/Database'
  use_frameworks!
  platform :watchos, '7.0'
end


post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
      config.build_settings['SWIFT_VERSION'] = '5.0'
    end
  end
end
