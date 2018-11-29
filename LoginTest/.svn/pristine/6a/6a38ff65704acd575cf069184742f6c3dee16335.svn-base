package com.service.impl;

import javax.annotation.Resource;

import org.springframework.stereotype.Service;
import org.springframework.transaction.annotation.Transactional;

import com.dao.UsersDAO;
import com.model.Users;
import com.service.UsersService;

/**
 * UsersService实现类
 * 
 * @author Administrator
 *
 */
@Service
@Transactional
public class UsersServiceImpl implements UsersService {
	@Resource
	private UsersDAO usersDAO;

	@Override
	public Users loginValidate(String username) {
		return usersDAO.findByUsername(username);
	}
}
