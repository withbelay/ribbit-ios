# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Ribbit' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Ribbit
pod 'FittedSheets'
pod 'TweeTextField'
pod 'Alamofire'
pod 'SSSpinnerButton'
pod 'DSFSparkline', :git => 'https://github.com/dagronf/DSFSparkline.git'
pod 'Charts'
pod 'Toast-Swift'
pod 'IQKeyboardManagerSwift'
pod 'BRYXBanner'
pod "KWVerificationCodeView"
pod 'SwiftyJSON'
pod 'ImageLoader'
pod 'SDWebImageSVGCoder'
pod "InitialsImageView"
pod 'SwiftyRSA'
pod 'AppCenter'

  target 'RibbitTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'RibbitUITests' do
    # Pods for testing
  end
end

post_install do |installer|
    installer.generated_projects.each do |project|
          project.targets.each do |target|
              target.build_configurations.each do |config|
                  config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
               end
          end
   end
end
