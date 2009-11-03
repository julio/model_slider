module ActiveRecord
  class Base
    def next
      self.class.first( 
        :conditions => ["created_at > ?", self.created_at],
        :order      => "created_at ASC")
    end
    def previous
      self.class.last( 
        :conditions => ["created_at < ?", self.created_at],
        :order      => "created_at ASC")
    end
  end
end
