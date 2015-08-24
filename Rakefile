require 'octokit'

@client = Octokit::Client.new(:access_token => ENV["GH_TOKEN"])
@client.auto_paginate = true

task :default do
  repos = @client.repos
  repos.map do |repo|
    prs = @client.pull_requests(repo.full_name, status: "open")
    puts "(#{prs.length}) #{repo.full_name}" if prs.length > 0

    prs.map do |pr|
      puts "    - #{pr.number} : #{pr.title} : #{pr.html_url}"
    end
  end
end

