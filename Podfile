platform :ios, '9.0'

use_frameworks!

def cocoa_pods
  pod 'Firebase/Core'
  pod 'Firebase/Auth'
  pod 'Firebase/Database'
  pod 'SVProgressHUD'
  pod 'ChameleonFramework'
end

target 'Ace Chat' do
  cocoa_pods
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['CLANG_WARN_DOCUMENTATION_COMMENTS'] = 'NO'
        end
    end
end