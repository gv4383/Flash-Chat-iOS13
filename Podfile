platform :ios, '10.0'

target 'Flash Chat iOS13' do
  use_frameworks!
  
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
      end
    end
    
    installer.pods_project.frameworks_group["iOS"]["MobileCoreServices.framework"].remove_from_project
  end

  # Pods for Flash Chat iOS13
  pod 'Firebase/Auth'
  pod 'Firebase/Firestore'
  
end
