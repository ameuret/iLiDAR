# Uncomment the next line to define a global platform for your project
# platform :ios, '15.6'

platform :ios, '15.4'

target 'iLiDARDepth' do
  pod 'CocoaAsyncSocket'
  pod 'AFNetworking'
  pod 'ReactiveCocoa', '~> 11.0'
  source 'https://github.com/CocoaPods/Specs.git'
  
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '15.4'
    end
  end
end
