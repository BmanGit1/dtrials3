class Micropost < ActiveRecord::Base

  attr_accessible :trial, :content  

  belongs_to :user  

  validates :trial, length: {maximum: 20 }

  validates :content, presence: true, length: { maximum: 140 }

  validates :user_id, presence: true

  default_scope order: 'microposts.created_at DESC'  #  descending order , newest first"

end
