# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'console-trouble'

  #↓これを入れると実行中のNSLogなどの出力がコンソールに出ません
  #app.info_plist['CFBundleName'] = "(ﾟ∀ﾟ)"

  app.codesign_certificate = ENV['CODESIGN_CERTIFICATE_DEV'] if ENV['CODESIGN_CERTIFICATE_DEV']
  app.provisioning_profile = ENV['PROVISIONING_PROFILE_DEV'] if ENV['PROVISIONING_PROFILE_DEV']
end
