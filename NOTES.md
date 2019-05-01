SELECT Users.name, Users.age, Pledges.amount
  FROM Pledges
  INNER JOIN Users
  ON Pledges.user_id = Users.id
  GROUP BY Users.id
  ORDER BY Users.name;